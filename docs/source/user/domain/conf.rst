Configurazione di Apache
========================

I web server di hosting `EWake <https://ewake.it>`_ utilizzano le configurazioni Apache del progetto `H5BP <https://h5bp.github.io>`_.
La versione del modulo H5BP attualmente utilizzata è scaricabile all'indirizzo https://public.ewake.it.

Inoltre è abilitato di default il modulo PageSpeed di Google, di cui si rimanda alla `documentazione ufficiale <https://developers.google.com/speed/pagespeed/module/>`_.


.htaccess di default
====================

Di seguito il codice del file *.htaccess* utilizzato in fase di creazione di ogni dominio ospitato presso `EWake <https://ewake.it>`_::

	# ##########################################################
	# PHP Values                                               #
	# ##########################################################
	
	php_value date.timezone Europe/Rome
	
	
	# ##########################################################
	# ModPagespeed                                             #
	# ##########################################################
	
	<IfModule pagespeed_module>
	
	
	# ----------------------------------------------------------
	# Configuration                                            |
	# ----------------------------------------------------------
	
	# ModPagespeed off
	
	# ModPagespeedAnalyticsID <Analytics ID>
	
	 
	# ----------------------------------------------------------
	# Core Filters                                             |
	# ----------------------------------------------------------
	# https://developers.google.com/speed/pagespeed/module/config_filters
	# Default: enabled.
	
	# Adds a <head> element to the document if not already present.
	# ModPagespeedDisableFilters add_head
	
	# Combines multiple CSS elements into one.
	# ModPagespeedDisableFilters combine_css
	
	# Combines multiple script elements into one.
	# ModPagespeedDisableFilters combine_javascript
	
	# Implied by recompress_images. Optimizes gifs to pngs.
	# ModPagespeedDisableFilters convert_gif_to_png
	
	# Adds a response header for each meta tag with an http-equiv attribute.
	# ModPagespeedDisableFilters convert_meta_tags
	
	# Converts larger jpegs to progressive format. Implied by recompress images.
	# ModPagespeedDisableFilters convert_jpeg_to_progressive
	
	# Producess lossy webp rather than jpeg images for browsers that support webp. Implied by recompress images.
	# ModPagespeedDisableFilters convert_jpeg_to_webp
	
	# Converts gif and png images into jpegs if they appear to be less sensitive to compression artifacts and lack alpha transparency. 
	# Implied by recompress images.
	# ModPagespeedDisableFilters convert_png_to_jpeg
	
	# Implied by rewrite_images. Replaces png and non-animated gif images with webp images on browsers that support the format.
	# ModPagespeedDisableFilters convert_to_webp_lossless
	
	# Extends cache lifetime of CSS, JS, and image resources that have not otherwise been optimized, by signing URLs with a content hash.
	# ModPagespeedDisableFilters extend_cache
	
	# Implied by extend_cache. Extends cache lifetime of otherwise unoptimized CSS resources by signing URLs with a content hash.
	# ModPagespeedDisableFilters extend_cache_css
	
	# Implied by extend_cache. Extends cache lifetime of otherwise unoptimized images by signing URLs with a content hash.
	# ModPagespeedDisableFilters extend_cache_images
	
	# Implied by extend_cache. Extends cache lifetime of otherwise unoptimized scripts by signing URLs with a content hash.
	# ModPagespeedDisableFilters extend_cache_scripts
	
	# Rewrites resources referenced in any CSS file that cannot otherwise be parsed and minified.
	# ModPagespeedDisableFilters fallback_rewrite_css_urls
	
	# Inline CSS by flattening all @import rules.
	# ModPagespeedDisableFilters flatten_css_imports
	
	# Implied by recompress_images. Reduces the color sampling of jpeg images to 4:2:0.
	# ModPagespeedDisableFilters jpeg_sampling
	
	# Inlines small CSS files into the HTML document.
	# ModPagespeedDisableFilters inline_css
	
	# Implied by rewrite_images. Replaces small images by data: urls.
	# ModPagespeedDisableFilters inline_images
	
	# Inlines <style> tags comprising only CSS @imports by converting them to equivalent <link> tags.
	# ModPagespeedDisableFilters inline_import_to_link
	
	# Inlines small JS files into the HTML document.
	# ModPagespeedDisableFilters inline_javascript
	
	# Implied by rewrite_images. Recompresses images, removing excess metadata and transforming gifs into pngs.
	# ModPagespeedDisableFilters recompress_images
	
	# Implied by recompress_images. Recompresses jpegs, removing excess metadata.
	# ModPagespeedDisableFilters recompress_jpeg
	
	# Implied by recompress_images. Recompresses pngs, removing excess metadata.
	# ModPagespeedDisableFilters recompress_png
	
	# Implied by recompress_images. Recompresses webps, removing excess metadata.
	# ModPagespeedDisableFilters recompress_webp
	
	# Implied by rewrite_images. Resizes images when the corresponding <img> tag specifies a smaller width and height.
	# ModPagespeedDisableFilters resize_images
	
	# Implied by rewrite_images. Resizes an image when the rendered dimensions of the image are smaller than the actual image.
	# ModPagespeedDisableFilters resize_rendered_image_dimensions
	
	# Rewrites CSS files to remove excess whitespace and comments, and, if enabled, rewrite or cache-extend images referenced in CSS files. 
	# In OptimizeForBandwidth mode, the minification occurs in-place without changing URLs.
	# ModPagespeedDisableFilters rewrite_css
	
	# Optimizes images, re-encoding them, removing excess pixels, and inlining small images. 
	# In OptimizeForBandwidth mode, the minification occurs in-place without changing URLs.
	# ModPagespeedDisableFilters rewrite_images
	
	# Rewrites JavaScript files to remove excess whitespace and comments. 
	# In OptimizeForBandwidth mode, the minification occurs in-place without changing URLs.
	# ModPagespeedDisableFilters rewrite_javascript
	
	# Implied by rewrite_javascript. Rewrites JavaScript external files to remove excess whitespace and comments. 
	# In OptimizeForBandwidth mode, the minification occurs in-place without changing URLs.
	# ModPagespeedDisableFilters rewrite_javascript_external
	
	# Implied by rewrite_javascript. Rewrites inline JavaScript blocks to remove excess whitespace and comments.
	# ModPagespeedDisableFilters rewrite_javascript_inline
	
	# Rewrite the CSS in style attributes if it contains the text 'url(' by applying the configured rewrite_css filter to it.
	# ModPagespeedDisableFilters rewrite_style_attributes_with_url
	
	# Implied by recompress_images. Strips color profile info from images.
	# ModPagespeedDisableFilters strip_image_color_profile
	
	# Implied by recompress_images. Strips EXIF meta data from images.
	# ModPagespeedDisableFilters strip_image_meta_data
	
	
	# ----------------------------------------------------------
	# OptimizeForBandwidth Filters                             |
	# ----------------------------------------------------------
	# https://developers.google.com/speed/pagespeed/module/optimize-for-bandwidth
	# Default: disabled.
	# CoreFilters: rewrite_css, rewrite_javascript, rewrite_javascript_external, rewrite_javascript_inline, convert_jpeg_to_progressive, convert_png_to_jpeg, convert_jpeg_to_webp, recompress_images, recompress_jpeg, recompress_png, recompress_webp, convert_gif_to_png, strip_image_color_profile, strip_image_meta_data, jpeg_sampling
	
	# Perform browser-dependent in-place resource optimizations. https://developers.google.com/speed/pagespeed/module/system#ipro
	# ModPagespeedEnableFilters in_place_optimize_for_browser
	
	
	# ----------------------------------------------------------
	# Experimental Filters                                     |
	# ----------------------------------------------------------
	# Default: disabled.
	
	# Adds JavaScript to page to measure latency and send back to the server.
	# ModPagespeedEnableFilters add_instrumentation
	
	# Redirects JavaScript libraries to a JavaScript hosting service.
	# ModPagespeedEnableFilters canonicalize_javascript_libraries
	
	# Removes excess whitespace in HTML files (avoiding <pre>, <script>, <style>, and <textarea>).
	# Default: enabled.
	# ModPagespeedDisableFilters collapse_whitespace
	
	# Combines multiple <head> elements found in document into one.
	# ModPagespeedEnableFilters combine_heads
	
	# Replaces animated gif images with webp images on browsers that support the format.
	# ModPagespeedEnableFilters convert_to_webp_animated
	
	# Replaces repeated inlined images with JavaScript that loads the image from the first occurence of the image.
	# ModPagespeedEnableFilters dedup_inlined_images
	
	# Defers the execution of JavaScript in HTML until page load complete.
	# ModPagespeedEnableFilters defer_javascript
	
	# Removes attributes which are not significant according to the HTML spec.
	# ModPagespeedEnableFilters elide_attributes
	
	# Implied by extend_cache. Extends cache lifetime of PDFs by signing URLs with a content hash.
	# ModPagespeedEnableFilters extend_cache_pdfs
	
	# Inserts Link:</example.css>; rel=preload headers to permit earlier fetching of important resources.
	# ModPagespeedEnableFilters hint_preload_subresources
	
	# Adds source maps to rewritten JavaScript files.
	# ModPagespeedEnableFilters include_js_source_maps
	
	# Inlines small CSS files used by fonts.googleapis.com into the HTML document.
	# Default: enabled.
	# ModPagespeedDisableFilters inline_google_font_css
	
	# Uses inlined low-quality images as placeholders which will be replaced with original images once the web page is loaded.
	# ModPagespeedEnableFilters inline_preview_images
	
	# Inserts <link rel="dns-prefetch" href="//www.example.com"> tags to reduce DNS resolution time.
	# Default: enabled.
	# ModPagespeedDisableFilters insert_dns_prefetch
	
	# Adds the Google Analytics snippet to each HTML page.
	# Default: enabled.
	# ModPagespeedDisableFilters insert_ga
	
	# Adds width and height attributes to <img> tags that lack them.
	# ModPagespeedEnableFilters insert_image_dimensions
	
	# Loads images when they become visible in the client viewport.
	# ModPagespeedEnableFilters lazyload_images
	
	# Cache inlined resources in HTML5 local storage.
	# ModPagespeedEnableFilters local_storage_cache
	
	# Convert synchronous use of Google Analytics API to asynchronous
	# ModPagespeedEnableFilters make_google_analytics_async
	
	# Convert synchronous use of Google AdSense API to asynchronous.
	# ModPagespeedEnableFilters make_show_ads_async
	
	# Moves CSS elements above <script> tags.
	# ModPagespeedEnableFilters move_css_above_scripts
	
	# Moves CSS elements into the <head>.
	# Default: enabled.
	# ModPagespeedDisableFilters move_css_to_head
	
	# Externalize large blocks of CSS into a cacheable file.
	# ModPagespeedEnableFilters outline_css
	
	# Externalize large blocks of JS into a cacheable file.
	# ModPagespeedEnableFilters outline_javascript
	
	# Add default types for <script> and <style> tags if the type attribute is not present and the page is not HTML5. 
	# The purpose of this filter is to help ensure that PageSpeed does not break HTML4 validation.
	# ModPagespeedEnableFilters pedantic
	
	# Replace CSS tags with inline versions that include only the CSS used by the page.
	# ModPagespeedEnableFilters prioritize_critical_css
	
	# Removes comments in HTML files (but not in inline JavaScript or CSS).
	# Default: enabled.
	# ModPagespeedDisableFilters remove_comments
	
	# Removes quotes around HTML attributes that are not lexically required.
	# ModPagespeedEnableFilters remove_quotes
	
	# Works just like inline_preview_images, but uses smaller placeholder images and only serves them to mobile browsers.
	# ModPagespeedEnableFilters resize_mobile_images
	
	# Makes images responsive by adding srcset with images optimized for various resolutions.
	# ModPagespeedEnableFilters responsive_images
	
	# Rewrites the domains of resources not otherwise touched by PageSpeed, based on MapRewriteDomain and ShardDomain settings in the config file.
	# ModPagespeedEnableFilters rewrite_domains
	
	# Rewrite the CSS in style attributes by applying the configured rewrite_css filter to it.
	# ModPagespeedEnableFilters rewrite_style_attributes
	
	# Combine background images in CSS files into one sprite.
	# ModPagespeedEnableFilters sprite_images
	
	# Shortens URLs by making them relative to the base URL.
	# ModPagespeedEnableFilters trim_urls
	
	</IfModule>

La file è scaricabile anche all'indirizzo https://public.ewake.it.

.. 
	attention (Attenzione)
	caution (Attenzione)
	danger (Pericolo)
	error (Errore)
	hint (Consiglio)
	important (Importante)
	note (Nota)
	tip (Suggerimento)
	warning (Avvertimento)
	admonition (non visibile)
	title (diventa il titolo della pagina)
.. attention:: Il filtro `insert_ga`, che è abilitato di default, sembra non funzionare con PHP in modalità PHP-FPM.


.user.ini di default
====================

Di seguito il codice del file *.user.ini* utilizzato in fase di creazione di ogni dominio ospitato presso `EWake <https://ewake.it>`_::

	;date.timezone = 'Europe/Rome'

	;display_errors = On
	
	; All
	;error_reporting = -1
	
	; Complete error reporting
	;error_reporting = 8191 
	
	; E_ALL ^ E_DEPRECATED ^ E_STRICT (alias of E_ALL & ~E_DEPRECATED & ~E_STRICT)
	;error_reporting = 22527
	
	; E_ALL ^ E_DEPRECATED ^ E_NOTICE (alias of E_ALL & ~E_DEPRECATED & ~E_NOTICE)
	;error_reporting = 22519
	
	; Zend error reporting
	;error_reporting = 128 
	
	; Basic error reporting
	;error_reporting = 8 
	
	; Minimal error reporting
	;error_reporting = 1

La file è scaricabile anche all'indirizzo https://public.ewake.it.

.. 
	attention (Attenzione)
	caution (Attenzione)
	danger (Pericolo)
	error (Errore)
	hint (Consiglio)
	important (Importante)
	note (Nota)
	tip (Suggerimento)
	warning (Avvertimento)
	admonition (non visibile)
	title (diventa il titolo della pagina)
.. attention:: Il file d `..user.ini` viene utilizzato solo con PHP in modalità CGI o FastCGI; ed ha un tempo di cache di **300 secondi**.


robots.txt di default
=====================

Di seguito il codice del file *robots.txt* utilizzato in fase di creazione di ogni dominio ospitato presso `EWake <https://ewake.it>`_::

	# www.robotstxt.org/
	
	# Allow crawling of all content
	User-agent: *
	Disallow:

La file è scaricabile anche all'indirizzo https://public.ewake.it.
