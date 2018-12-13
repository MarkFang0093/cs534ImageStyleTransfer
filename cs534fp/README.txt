To run just style transfer:
	put base images ended with .jpg in domo/output3/ and style image in style/style.jpg
	output is in output4/
	multiple picture per run is ok
	in detectron/ type: ''
	to execute
	python3.5 is recommended
to run partial style transfer
	in this case, anything that is not recognized by detectron ie the background will not
	be style transfered.
	put base images ended with .jpg in domo and style image in style/style.jpg
	output is in output4/
	multiple picture per run is ok
	in detectron/ type: 'sh run.sh'

weight of the content, style and even iterations in network user want to modify can be altered in
style_transfer/Style-Transfer.py line 431
    img.append(style_transfer(base_list[i], style_image, content_layer_ids,style_layer_ids, 2.0, 10.0, 0.3, 100, 10.0)) ;
the default for content is 2.0 and default for style is 10.0 and default for iteration is 100 which can all be adjucted by user

detectron is modified from the oringinal to fit in the need of this project

 
