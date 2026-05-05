// Consulta básica
db.productos.find()

//Consulta con filtro
db.productos.find({ marca: "Samsung" })

// Consulta con condición
db.productos.find({ precio: { $gt: 2000000 } })


// Consulta combinada
db.productos.find({
  marca: "Apple",
  precio: { $gt: 3000000 }
})

// Actualización
db.productos.updateOne(
  { nombre: "iPhone 15" },
  { $set: { precio: 3900000 } }
)

// Eliminación
db.productos.deleteOne({ nombre: "M170" })


// Agregación (conteo)
db.productos.aggregate([
  { $count: "total_productos" }
])


// Agregación (conteo)
db.productos.aggregate([
  { $count: "total_productos" }
])


// Agregación (promedio)
db.productos.aggregate([
  {
    $group: {
      _id: "$marca",
      promedio: { $avg: "$precio" }
    }
  }
])


//Agregación (suma)
db.productos.aggregate([
  {
    $group: {
      _id: null,
      total: { $sum: "$precio" }
    }
  }
])