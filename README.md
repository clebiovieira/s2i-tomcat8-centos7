# s2i-tomcat8-centos7
openshift s2i build tomcat8 application
## 编译image
* docker build <your docker registry>imagename:tag  .
* docker push <your docker registy>imagename:tag 
* 修改template 文件夹下的s2i-tomcat8-centos7.json,注意buildconfig下的from namespce 和name,这2个是你刚才push到仓库的image,其他的根据自己需要修改。
## 创建模版
* oc ceate -f s2i-tomcat8-centos7.json 
* 创建模版时可以在模版的annotations 下加入tag：quickstart ,java 这样模版会被归类到java 分类中。

 
