using System;
using System.Collections.Generic;
using System.Linq;
namespace GestionProductos
{
public class Producto
{
\\Codigo de la clase Producto igual que antes
pulic class Almacen
{
private List<Producto>productos=newList<Producto>();
public bool
AgregarProducto(Producto p)
{
if(productos.Any(prod=>prod.Codigo==p.Codigo))return false;
productos.Add(p)
return true;
}
public List<Producto>
BuscarProducto(string criterio)
{
criterio=criterio.ToLower();
return productos.Where(p=>p.Codigo.ToLower().Contains(criterio)||p.Nombre.ToLower().Constains(criterio)).ToList();
}
public bool EliminarProducto(string codigo)
{
var producto=productos.FirstOrDefault(p=>p.Codigo==codigo);
if(producto==null) return false;
productos.Remove(producto(;
return true;
}
}
}

