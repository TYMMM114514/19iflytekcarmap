#19iflytekcarmap
地图导入gazebo

打开gazebo 选择左上角的Edit->Model Editor

点击custom shapes下面的add 找到map的对应路径 选择19iflytekditu.dae

把地图放置在gazebo中 并点击左上的Model 选中static

ctrl + s保存文件 路径随意 退出gazebo

打开保存的路径 打开文件夹中的model.sdf 删除

        <material>
          <lighting>1</lighting>
          <script>
            <uri>file://media/materials/scripts/gazebo.material</uri>
            <name>Gazebo/Grey</name>
          </script>
        </material>
打开gazebo 点击Insert 找到保存的文件 添加地图

将地图保存为world文件

可以删除gazebo中自带的ground_plane让地板贴图清晰（好像有点问题只能从底下看）