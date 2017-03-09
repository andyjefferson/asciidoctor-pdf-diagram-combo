# asciidoctor-pdf-diagram-combo
Example of using Asciidoctor generating PDF using asciidoctor-diagram


I'm wanting to use Asciidoctor to generate a site in HTML, and also PDF, and using Maven.

This works fine until I want to generate diagrams using the asciidoctor-diagram plugin. 
The HTML site is still generated fine with the generated images for the diagrams.
The PDF site always spits out messages like

    asciidoctor: WARNING: image to embed not found or not readable: /home/andy/work/test/asciidoctor-pdf-diagram-combo/src/main/asciidoc/sub/relation_1_1_uni_db.png

since the PDF plugin is looking in the source tree only for images, and the generated image is in the target/site area.

I don't want to generate the diagram images in the source tree (since don't want them checked in).
