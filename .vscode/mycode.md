# gallery script include
{% include image-gallery.html folder="/uploads/album" %}

# convert jpg to png, for gallery script
for f in ./*.jpg ; do convert "$f" -resize 500x400 "${f%.jpg}.webp" ; done

