# git 的使用

## 基本的配置

git config --global user.name "注册名"

git config --global user.email "注册邮箱"

> 这些是提交后显示的

`生成ssh`
ssh-keygen -t rsa -C "自己的邮箱"
一路默认就行过程中会告诉ssh存放位置

之后我们拿着公钥即.pub 设置github setting中的ssh

`测试连接`
`ssh -T git@github.com`
中途会警告无关紧要

## 推送文件

### 建立本地仓库

> 第一种方式

- 新建文件夹
- 在git bash 中打开即右键
- `git init` 之后会出现`.git`文件夹

> 第二种方式

- 先克隆远程库: `git clone git@github.com:用户名/仓库名.git`

> 1.add
> 使用方法
> git add 单个文件
> git add 文件夹/
> git add 文件夹1/ 文件夹2/   多个文件夹
> git . 当前整个仓库
---

> 2.commit
> `git commit -m "注释"`

---

> 3.push
> `git push -u origin main 或 main`

以上是简略版
