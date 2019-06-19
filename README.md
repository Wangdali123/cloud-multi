# cloud-multi
这是一个多模块的主项目，子模块有各自的git地址<br>
v0.1测试主项目包含子项目的结构<br>
v0.2测试多模块提交（验证包含子项目是否成功）

**** 
## 多模块项目
### 普通项目创建
1. 先创建maven父项目,类型选择maven-archetype-quickstart。
2. 右键>New>Module>选择子模块项目类型。
3. 删除父项目的src目录，保留pom.xml。子模块pom与父pom无依赖，父项目就类似一个工作区间。
### 多git项目创建
#### 父子模块有依赖关系
1. 创建maven父项目,类型选择maven-archetype-quickstart，删除src目录，git初始化>创建提交。
2. 新建一个项目，初始化>创建提交。
3. 将子项目copy到父项目目录。
4. New>Project Structure>Modules>（+）>Import Module>选择主仓库目录>maven>选择search for projects recursively和Import Maven projects automatically>>...。
5. 点击git>Repository>Remotes>此时可以看到多个git路径。
6. git push代码时可以选择不同项目。
#### 父工作区间
1. 模块平级的只需要创建一个本地工作区间
2. 平级：new>Project from xx直接导入
