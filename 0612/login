login

@app.route('/login')
def login():
    head, level, page = parse_content()
    directory = render_menu(head, level, page)
    if not isAdmin():
        return set_css()+"<div class='container'><nav>"+ \
    directory+"</nav><section><h1>Login</h1><form method='post' action='checkLogin'> \
    Password:<input type='password' name='password'> \
    <input type='submit' value='login'></form> \
    </section></div></body></html>"
    else:
        return redirect('/edit_page')


    
定義：login
由開頭、頁數等加起來等於組成內容
目錄等於給予開頭頁數的畫面
如果你不是管理者
    就會回到建立css
    登入密碼等於密碼的名字也就是登入介面的標題。
    