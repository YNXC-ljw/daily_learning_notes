# Git的使用

## 1. 在本地文件下创建git仓库

```bash
git init
```
<img width="661" height="104" alt="image" src="https://github.com/user-attachments/assets/ba8360bf-e11b-4d20-a5df-100187f40fae" />

## 2. 配置本地仓库的一些属性如email和name

如果不配置email和name，那么在将文件提交到仓库中时会出现一系列的问题，所以在创建仓库时，一定要先配置一下email和name

```bash
用户名：git config user.name "用户名"
邮箱：git config user.email "邮箱"
查看仓库信息：git config -l
```
<img width="1237" height="363" alt="image" src="https://github.com/user-attachments/assets/a40b01c0-7031-4b2a-8562-fe0602ae476d" />

```bash
删除重置用户名：git config --unset user.name
删除重置邮箱：git config --unset user.email
```

<img width="1015" height="283" alt="image" src="https://github.com/user-attachments/assets/8bfc8659-beb5-49ea-b775-bf3d7d274431" />

**还有一个比较重要的选项**，它的作用是使设置的该信息(用户名或邮箱)在服务器上所有的git仓库都有效，因为一个机器上是可以创建多个仓库的。当然，想要重置删除全局信息也是需要加上该选项

```bash
--global
用户名：git config --global user.name "用户名"
邮箱：git config --global user.email "邮箱"
```
