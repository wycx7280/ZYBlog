# ZYBlog
a program for personal management

1. 数据库设计： (只列出关键字, 其他自己补充, 不对告诉我一声, 都在这个文档里定义修改)
   1. 用户表： id password name email
   2. 博客表： id content created_by(用户id当作外键), 点赞数, 评论数
   3. 点赞表:  (联合主键：user_id blog_id) time
   4. 字幕表:  (联合主键：user_id blog_id) content
   5. 评论表:  (联合主键：user_id blog_id) content
   6. 文档表:  id doc_path co_user(协作人)
   7. 协作信息表： doc_id  add_time co_info 是否完成
2.  要求：
   1. 字段名自己设计规则定义, 必须有说明书
   2. 数据库使用mysql
   3. 后端使用Java Spring 
   3. 使用redis做优化
