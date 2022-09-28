# sca-day-3-project
 Rendering HTML Templates - Serving Static Files

You've downloaded a template and you want to integrate it into your app
- Put the base html file inside the templates folder of your app as usual
- Define your view function, urls of the app and add the path to the core urls as usual
- Create a 'static' folder and put the assets,images,scss and so on from the downloaded template into it
- In core/settings.py, add STATICFILES_DIRS = [BASE_DIR/'STATIC'] under STATIC_URL line
- Go back to your html file and add "{% static  %}" to every external file reference
E.g. src="images/portfolio/portfolio-5.jpg" will now become src="{% static "images/portfolio/portfolio-5.jpg" %}"
    src="assets/vendors/js/glightbox.min.js"  will now become src="{% static "assets/vendors/js/glightbox.min.js" %}"