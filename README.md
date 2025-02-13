import flet as ft
def main (page: ft.Page):
    page.window_center()
    page.bgcolor = '#17b8cb'
    page.window_width = '1000'
    page.window_height = '600'
    page.window_resizable = False
    page.window_maximizable = False
    r1= ft.Row([
        ft.Container(
        bgcolor='#ffffff',
        width=450,
        height=540,
        border_radius= 5,
        padding=30,
        content= ft.Column ([  
        ft.Text("Faça seu  Login", size = 35),
        ft.TextField(label ='E-mail', icon= ft.icons.ACCOUNT_BOX),
        ft.TextField(label ='Senha', icon= ft.icons.ACCOUNT_BOX,  password = True, can_reveal_password = True),
        ft.FilledTonalButton (content=ft.Text('Entrar') ,width = '250', height=50, style=ft.ButtonStyle(bgcolor='#17b8cb',color='#ffffff')
                              ,on_click= lambda e: entrar (e )),
        ft.TextButton(text="Esqueceu a senha?", on_click= True),
        ft.TextButton('Não tem conta?Fazer cadastro?',width=300)
        
 
