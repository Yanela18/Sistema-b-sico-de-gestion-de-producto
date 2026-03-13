using System;
using System.Collections.Generic;
namespace GestionProducto
{
public string Codigo{get;set;}
public string Nombre{get;set;}
public decimal Precio{get;set;}

public Producto(string codigo,string nombre, decimal precio)
{
Codigo=codigo;
Nombre=nombre;
Precio=precio;
}
public override string ToString()=>$"Codigo:{Codigo}, Nombre:{Nombre}, Precio:{Precio:C}";
}
public class Almacen
{
private List<Producto>productos= new List<Producto>();
}
}
