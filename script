// Espera a que el DOM esté completamente cargado
document.addEventListener("DOMContentLoaded", function() {
    // Obtiene todos los enlaces del menú de navegación
    var navLinks = document.querySelectorAll("nav ul li a");

    // Agrega un evento de clic a cada enlace del menú de navegación
    navLinks.forEach(function(navLink) {
        navLink.addEventListener("click", function(event) {
            // Evita el comportamiento predeterminado del enlace
            event.preventDefault();

            // Obtiene el valor del atributo href del enlace
            var targetId = this.getAttribute("href").substring(1);

            // Busca el elemento en la página con el ID correspondiente
            var targetElement = document.getElementById(targetId);

            // Si se encuentra el elemento, realiza un desplazamiento suave hacia él
            if (targetElement) {
                var targetPosition = targetElement.getBoundingClientRect().top + window.pageYOffset;
                window.scrollTo({
                    top: targetPosition,
                    behavior: "smooth"
                });
            }
     
