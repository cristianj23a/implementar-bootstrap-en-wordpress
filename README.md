# implementar-bootstrap-en-wordpress

Ruta: public_html/wp-content/themes/"Tema que usas"/functions.php

// Incluir Bootstrap CSS
```
function bootstrap_css() {
- wp_enqueue_style( 'bootstrap_css', 
       get_stylesheet_directory_uri() . '/css/bootstrap.min.css', 
       array(), 
       '4.0.0'
       ); 
}
add_action( 'wp_enqueue_scripts', 'bootstrap_css');
```

// Incluir Bootstrap JS
```
function bootstrap_js() {
 wp_enqueue_script( 'bootstrap_js', 
       get_stylesheet_directory_uri() . '/js/bootstrap.min.js', 
       array('jquery'), 
       '4.0.0', 
       true); 
}
add_action( 'wp_enqueue_scripts', 'bootstrap_js');
```
