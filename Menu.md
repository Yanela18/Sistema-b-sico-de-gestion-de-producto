using System;
using System.Collections.Generic;
using System.Linq;

namespace GestionProductos
{
    public class Producto
    {
        // Código de la clase Producto igual que antes
    }

    public class Almacen
    {
        // Código de la clase Almacen igual que antes
    }

    class Program
    {
        static void Main()
        {
            var almacen = new Almacen();
            bool salir = false;

            while (!salir)
            {
                Console.Clear();
                Console.WriteLine("=== Menú de Gestión de Productos ===");
                Console.WriteLine("1. Registrar producto");
                Console.WriteLine("2. Buscar producto");
                Console.WriteLine("3. Eliminar producto");
                Console.WriteLine("3. Eliminar producto");
                Console.WriteLine("4. Listar productos");
                Console.WriteLine("5. Salir");
                Console.Write("Seleccione una opción: ");

                switch (Console.ReadLine())
                {
                    case "1": RegistrarProducto(almacen); break;
                    case "2": BuscarProducto(almacen); break;
                    case "3": EliminarProducto(almacen); break;
                    case "4": ListarProductos(almacen); break;
                    case "5": salir = true; break;
                    default:
                        Console.WriteLine("Opción no válida.");
                        Console.ReadKey();
                        break;
                }
            }
        }

        static void RegistrarProducto(Almacen almacen)
        {
            // Código para registrar producto
        }

        static void BuscarProducto(Almacen almacen)
        {
            // Código para buscar producto
        }

        static void EliminarProducto(Almacen almacen)
        {
            // Código para eliminar producto
        }

        static void ListarProductos(Almacen almacen)
        {
            // Código para listar productos
        }
    }
}
