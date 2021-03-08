# FlexBox-Menu-icon-Dropdown
Menú FlexBox. Icono Redes Sociales. Menú DropDown
```javascript
/* Dropdown */
.dropdown ul {
    display: flex;
    flex-direction: column;
} 
@media screen and (min-width:760px) {
    .dropdown ul {        
        flex-direction: row;
    } 
}
.dropdown ul li {
    display: flex;    
    flex-direction: column;
}

@media screen and (min-width:760px) {
    /* Para poder crear el SubMenú */
    .dropdown ul li {
        position: relative;
        display: flex;
        flex: 1 1 100%;
        
    }
    .dropdown ul li ul {
        position: absolute;
        top: 100%;  
        left: 0;  /*Sub menu alinear a la izquierda*/    
        background-color: #334bd3;
        display: none; /*para esconder sub menu*/
        width: 100%;/*SubMenu tengo =ancho que Padre*/
        
    }
    .dropdown ul li:hover ul {
        display: flex;
        flex-direction: column;
    }
}

/* Redes Sociales */
.sociales ul li span {
    display:none;
}
.sociales ul {
    display: flex;
    justify-content: flex-end;
}
.sociales ul li a:before {
    /* La forma que se carga FonAwesome en la hoja de estilos */
    /* Esto habilita los enlaces utilicen los iconos de FontAwesome */
    font-family: "Font Awesome 5 Brands";
}
.sociales ul li a[href*='facebook.com']::before {
    content: "\f39e";
}
.sociales ul li a[href*='twitter.com']::before {
    content: "\f099";
}
.sociales ul li a[href*='youtube.com']::before {
    content: "\f167";
}
.sociales ul li a[href*='instagram.com']::before {
    content: "\f16d";
}
.sociales ul li a[href*='github.com']::before {
    content: "\f09b";
}

/* Sociales y DropDown */
.nav-social-dropdown {
    display: flex;
    justify-content: space-between;
    background-color: #152370;
}
```
