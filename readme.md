# Apartado obligatorio
## Código HTML

Creamos el contenido principal "main", en el que añadimos el título H2, y creamos un container-main con sus respectivas divisiones en div, en el que se incluye la foto, la descripción y el precio:

<main class="main">
    <h2 class="titulo">NUEVAS COLECCIONES</h2>
    <div class="container-main">
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-3.jpg" alt="Vestido celeste" title="Vestido celeste">
            <div class="PrecioProducto">
                <span class="Producto">Vestido</span>
                <span class="Precio">34,99 €</span>
            </div>
        </div>
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-6.jpg" alt="Camisa amarilla" title="Camisa amarilla">
            <div class="PrecioProducto">
                <span class="Producto">Camisa</span>
                <span class="Precio">44,99 €</span>
            </div>
        </div>
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-4.jpg" alt="Vaqueros" title="Vaqueros">
           <div class="PrecioProducto">
                <span class="Producto">Vaqueros</span>
                <span class="Precio">79,99 €</span>
            </div>
        </div>
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-5.jpg" alt="Polo beige" title="Polo beige">
            <div class="PrecioProducto">
                <span class="Producto">Polo</span>
                <span class="Precio">44,95 €</span>
            </div>
        </div>
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-1.jpg" alt="Camisa blanco sucio" title="Camisa blanco sucio">
            <div class="PrecioProducto">
                <span class="Producto">Camisa</span>
                <span class="Precio">25,00 €</span>
            </div>
        </div>
        <div class="item">
            <img class="img" src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/images/image-2.jpg" alt="Camiseta blanca" title="Camiseta blanca">
            <div class="PrecioProducto">
                <span class="Producto">Camiseta</span>
                <span class="Precio">22,99 €</span>
            </div>
        </div>
    </div>
    </main>

## Código CSS

- Para main, aplicamos un padding para separarlo del menú de navegación y del footer. definimos el estilo del título.
.main {
  padding: 16px;
}
.titulo {
  font-family: "Montserrat", sans-serif;
  font-size: 32px;
  font-weight: bold;
}
- Aplicamos display grid a container-main que es donde tenemos clasificados los items, así como márgenes y el formato columnas.
.container-main {
  display: grid;
  max-width: 1280px;
  grid-template-columns: repeat(3, 1fr);
  margin-left: 110px;
  margin-right: 110px;
  margin-bottom: 32px;
  gap: 64px;
  background-color: var(--primary);
}
- A cada item (foto y su precio), le añadimos display flex - column, a la imagen, borde.
.item {
  display: flex;
  flex-direction: column;
  gap: 32px;
}
.img {
  border-radius: 16px;
}
- También le damos formato a la descripción y al precio.
.PrecioProducto {
  font-size: 14px;
  font-family: "Montserrat", sans-serif;
  display: flex;
  margin-left: 24px;
  margin-right: 24px;
  justify-content: space-between;
}
.Precio {
  font-weight: bold;
}
.Producto {
  font-weight: normal;
}

# Apartado opcional

## Código HTML barra navegación
 <nav class="container-nav">
            <div class="item-nav1">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-menu-burguer.svg" alt="Desplegable">
            </div>
            <div class="item-nav2">
                <div class="menu1">
                <a href="Moda mujer">MODA MUJER</a>
                </div>
                <div class="menu2">
                <a href="Moda hombre">MODA HOMBRE</a>
                </div>
                <div class="menu3">
                <a href="Nueva colección">NUEVA COLECCIÓN</a>
                </div>
                <div class="menu4">
                <a href="Colecciones especiales">COLECCIONES ESPECIALES</a>
                </div>
            </div>
            <div class="item-nav3">
                <div class="imgnav2">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-user.svg" alt="Sign in">
                </div>
                <div class="imgnav3">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-heart.svg" alt="Wish list">
                </div>
                <div class="imgnav4">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-shopping-cart.svg" alt="Purchase">
                </div>
            </div>
    </nav>

## Código CSS barra navegación

- Añadimos display flex, con los respectivos formatos de estilo, así como position sticky y borde inferior
.container-nav {
  display: flex;
  background-color: white;
  font-size: 16px;
  font-weight: normal;
  padding: 32px;
  justify-content: space-between;
  border-width: 0px 0px 0.9px 0px;
  border-bottom-color: var(--secondary);
  border-style: solid;
  position: sticky;
  top: 0;
}
- A los items de la barra de navegación, del menú principal e iconos de la derecha, le añadimos display grid.
.item-nav2 {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

.item-nav2 a {
  color: var(--secondary);
  text-decoration: none;
}
.item-nav3 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 40px;
}

## Código HTML footer

- El footer lo dividimos en diferentes div con su imagen y texto correspondiente.
<footer>
        <div class="container-footer">
            <div class="item-footer">
                <div class="imgfooter">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-truck.svg" alt="Entrega">
                </div>
                Entrega
            </div>
            <div class="item-footer">
                Devoluciones y cambios
            </div>
            <div class="item-footer">
                <div class="imgfooter">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-phone.svg" alt="Teléfono">
                </div>
                +375 (29) 749-18-23
            </div>
            <div class="item-footer">
                <div class="imgfooter">
                <img src="https://raw.githubusercontent.com/Lemoncode/fotos-ejemplos/main/online-shop/icons/icon-mail.svg" alt="Email">
                </div>
                shop@omix.com
            </div>
        </div>
    </footer>

## Código CSS footer

- Le añadimos display flex, le damos diferentes formatos requeridos, a la imagen le aplicamos un border radius y al item un align items center.
.container-footer {
  display: flex;
  padding: 32px;
  justify-content: space-between;
  font-size: 16px;
  font-weight: normal;
  color: var(--primary);
  background-color: var(--secondary);
}
.imgfooter {
  background-color: var(--primary);
  border-radius: 64px;
  padding: 8px;
  margin-right: 16px;
}
.item-footer {
  display: flex;
  align-items: center;
}

# Apartado extra

## Código CSS ancho pantalla

@media (max-width: 920px) {
  .container-footer {
    flex-direction: column;
    gap: 32px;
  }
  .item-footer {
    padding-bottom: 16px;
    border-bottom: 1px solid var(--primary);
  }
  .item-nav1 {
    margin: 0 auto;
  }
  .item-nav2 {
    display: none;
  }
  .item-nav3 {
    display: none;
  }
  .container-main {
    grid-template-columns: repeat(1, 1fr);
  }
}
