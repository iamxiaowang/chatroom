
"""
    python实现网络聊天室
    版本(v1.0)
"""

功能说明：

    1.利用图形界面：如，tkinter GUI 实现用户操作

    2.用户登录和注册：
        
        *打开客户端，客户端初始化，连接成功服务器，进入登录，注册界面
        *客户端点击注册，用户填写账号，用户进行设置密码，确认密码，昵称，缺一不可，将信息发送给服务起处理
         不符合安全等级要求，需客户重新输入密码，用户账号唯一
        *登录成功之后，服务器长期保存用户信息.用户进入聊天界面
        *客户凭借用户名，密码可实现再次登陆,登陆后进入聊天界面
        *账号只能在一处登入，在别处登入时把原来登陆的踢下线

    3.好友跟群管理:
        *用户通过主界面点击添加好友的按钮，弹出加好友框，输入好友账号进行添加，通过对方同意后即成为好友
        *用户通过主界面点击创建群，弹出创建群框，输入群号，即可创建群，群号唯一
        *用户通过主界面点击加入群，弹出加群框，输入群号，即可加入聊天群

    ４.聊天模块需求：
        *支持群聊功能、私聊，加群、创建群的功能
        *聊天界面显示好友列表，聊天窗口，通过点击好友或群聊昵称切换聊天界面
        *有加好友功能，对方收到通知，通过/拒绝/推迟到下次登入时询问
        *用户再次打开时恢复所有聊天记录，（用户离线时收到的未读的消息有红点提示或有未读信息用数字统计显示）
        *在线好友表显示蓝色，离线好友显示灰色，实时显示并实时更新用好友在线状态
        *支持用户通过在聊天窗口，进行图片传输,文件转发，文件下载操作
        *对聊天内容涉及敏感词汇过滤处理，并能发出警告
        *用户通过加群号进入群时，群里会收到某某进群的消息提示
        *使用数据库存储用户信息、好友关系、群成员、所有聊天记录
        *群聊中显示群成员（双击打开聊天窗口/发送好友请求）；实时显示群成员在线状态，置顶在线的成员
        *联系人列表中的显示最近消息（同QQ，群聊则显示发送者昵称，图片则显示[图片消息]，自动处理换行）
        *可增加获取天气的信息的功能
        
        
    5.数据库设计：
        用户信息表user
        聊天记录表chat_history
        好友表:friends
        聊天室:rooms
        聊天室用户:room_user

    6.设计文件说明
            ├── client
        │   ├── client.py
        │   └── connfig.py
        ├── demand
        │   ├── client_mind.png
        │   ├── demand.png
        │   ├── io_client_server
        │   ├── mysql_design
        │   ├── server_mind.png
        │   └── ui_client
        ├── demand_analyze
        ├── README.md
        ├── server
        │   ├── connfig.py
        │   ├── __pycache__
        │   │   ├── connfig.cpython-35.pyc
        │   │   ├── response.cpython-35.pyc
        │   │   ├── server_tool.cpython-35.pyc
        │   │   ├── sql_db.cpython-35.pyc
        │   │   └── sql_tool.cpython-35.pyc
        │   ├── response.py
        │   ├── server_main.py
        │   ├── server_tool.py
        │   ├── sql_db.py
        │   └── sql_tool.py
        └── ui
            ├── backgr.gif
            ├── client_main.py
            └── tkinter01.py



        
        
