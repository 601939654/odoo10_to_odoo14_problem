# odoo10转odoo14问题记录
1、_init_.py文件中的import写法改为from . import

2、action定义里面没有<field name="view_type">form</field>

3、没有了@api.multi装饰器，直接删除

4、form视图中的lable标签需要指定for=“field name”

5、tre视图的列表颜色控制，没有了color属性写法，改为如下：

  红色：decoration-danger="name=='decoration-danger'"
  蓝色：decoration-info="name=='decoration-info'"
  灰色：decoration-muted="name=='decoration-muted'"
  默认颜色（紫色）：decoration-primary="name=='decoration-primary'"
  绿色：decoration-success="name=='decoration-success'"
  橙色：decoration-warning="name=='decoration-warning'"
