# Ferreter-a-El-Tornillo-Feliz

Ferretería El Tornillo Feliz
from tkinter import *

#creamos la ventana

ventana = Tk()
ventana.geometry('720x680')
ventana.resizable(width = False, height = False )
ventana.configure(bg = 'gray90')

# título

ventana.title("Ferretería El Tornillo Feliz")

# Creamos el Título

TextoTitulo = Label(ventana, text = ' Ferretería El Tornillo Feliz', bg = 'gray90',fg = 'gray9', font=("Sitka Small", 25, "italic"))
TextoTitulo.pack(pady=10)

# Creamos los primeros textos con sus respectivas cajas de texto

TextoDNI = Label(ventana, text = 'DNI: ', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 20, y = 60)
CajaDNI = Entry(ventana, bg = 'white', fg = 'gray9',font = '15',border = '2').place(x = 140, y = 60, width = 200, height = 30)

TextoApellidos = Label(ventana, text = 'Apellidos: ', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 20, y = 100)
CajaApellidos = Entry(ventana, bg = 'white', fg = 'gray9', font = '15', border = '2').place( x = 140, y = 100, width = 200, height = 30)

TextoNombre = Label(ventana, text = 'Nombres: ', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 380, y = 100)
CajaANombre = Entry(ventana, bg = 'white', fg = 'gray9', font = '15', border = '2').place( x = 470, y = 100, width = 200, height = 30)

TextoDireccion = Label(ventana, text = 'Direccion: ', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 20, y = 140)
CajaDireccion = Entry(ventana, bg = 'white', fg = 'gray9', font = '15', border = '2').place( x = 140, y = 140, width = 400, height = 30)

TextoTelefono = Label(ventana, text = 'Telefono: ', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 20, y = 180)
CajaTelefono = Entry(ventana, bg = 'white', fg = 'gray9', font = '15', border = '2').place( x = 140, y = 180, width = 400, height = 30)

# Títulos de las Tablas del producto 

TextoCod_Prod = Label(ventana , text = 'Cod_prod', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x =20, y = 240)
TextoDescripcion = Label(ventana, text = 'Descripción', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 115, y = 240)
TextoUnidad = Label(ventana, text = 'Unidad', bg = 'gray90',fg = 'gray9', font=("Arial", 13)).place(x = 220, y = 240)
TextoCantidad = Label(ventana, text = 'Cantidad', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 290, y = 240)
TextoPrecio = Label(ventana, text = 'Precio',bg = 'gray90',fg = 'gray9', font=("Arial", 13)).place(x = 380, y = 240)
TextoSubtotal = Label(ventana, text = 'Subtotal', bg = 'gray90', fg = 'gray9', font=("Arial", 13)).place(x = 450, y = 240)

# Cajas de Cod_Prod

CejaCod_Prod1 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 20, y = 280, width = 80, height = 25)
CejaCod_Prod2 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 20, y = 320, width = 80, height = 25)
CejaCod_Prod3 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 20, y = 360, width = 80, height = 25)

# Cajas de Cantridad

CejaCantidad1 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 290, y = 280, width = 80, height = 25)
CejaCantidad2 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 290, y = 320, width = 80, height = 25)
CejaCantidad3 = Entry(ventana, bg = 'white', fg = 'gray9', font = '10', border = '2').place(x = 290, y = 360, width = 80, height = 25)

# Total Ventana

TextoPrecio = Label(ventana, text = 'Total', bg = 'gray90', fg = 'gray9',   font=("Sitka Small", 20)).place(x = 600, y = 400)

# Botones

BotonGuardar = Button(ventana, text = 'Guardar',bg = 'green2', fg = 'white', font= '"Verdana" 12', border = '0', activebackground="green yellow",borderwidth = 15).place(x = 180, y = 460, width = 250, height = 50)
BotonImprimir = Button(ventana, text = 'Imprimir', bg = 'green2', fg = 'white', font = '"Verdana" 12', border = '0',activebackground="green yellow", borderwidth = 15).place(x = 450 , y = 460, width = 250, height = 50)

ventana.mainloop()



