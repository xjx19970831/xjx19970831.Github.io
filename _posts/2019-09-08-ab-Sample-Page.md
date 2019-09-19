---
title: vue案例
published: true　　
---
   
## vue，前端常用框架。
  vue格式：   
    
     ```var v=new Vue({
         el:挂载点，
         data:{},
         method:{}
     })

用vue格式去使用element ui的插件


```
vue修改的代码
 <body>
		<div id="x">
			<el-upload 
				action="图片上传的目的地" 
				list-type="picture-card" 
				:on-preview="handlePictureCardPreview" 
				>
				<i class="el-icon-plus"></i>
			</el-upload>
			<el-dialog :visible.sync="dialogVisible">
				<img width="100%" :src="dialogImageUrl" alt="">
			</el-dialog>
		</div>
		<script>
			var v = new Vue({
				el:"#x",
				data:{
					dialogImageUrl: '',
					dialogVisible: false
				},
				methods:{
					handlePictureCardPreview:function(file) {
						this.dialogImageUrl = file.url;
						this.dialogVisible = true;
					}
				}
			});
		</script>
	</body>

``` 

饿了么代码
<el-upload
  action="https://jsonplaceholder.typicode.com/posts/"
  list-type="picture-card"
  :on-preview="handlePictureCardPreview"
  :on-remove="handleRemove">
  <i class="el-icon-plus"></i>
</el-upload>
<el-dialog :visible.sync="dialogVisible">
  <img width="100%" :src="dialogImageUrl" alt="">
</el-dialog>
<script>
  export default {
    data() {
      return {
        dialogImageUrl: '',
        dialogVisible: false
      };
    },
    methods: {
      handleRemove(file, fileList) {
        console.log(file, fileList);
      },
      handlePictureCardPreview(file) {
        this.dialogImageUrl = file.url;
        this.dialogVisible = true;
      }
    }
  }
</script>