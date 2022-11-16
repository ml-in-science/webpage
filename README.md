## Repo for the Machine Learning in Science colloquium [webpage](https://ml-in-science.github.io/webpage) at the University of Glasgow

You need the correct venv to render the .ipynb to .html. Use the "pkg.txt" file in this repo to create and environment. Easiest to do with Anaconda (https://www.anaconda.com/).
Just open anaconda prompt and type "conda create --name MLiS --file pkgs.txt" (The MLiS can be whatever name you want to give it). Then use "conda activate MLiS" and finally "jupyter notebook".

Notes:
	- get rid of table hovering color by commenting out ".rendered_html tbody tr:hover" in html file
	- show the contents of first cell and bring back "in[]/out[]" prompt margins by opening the .ipynb 
	  file in VScode and looking for first cell contents: 
		"source": [
 		   "from IPython.core.display import display,HTML\n",
 		   "display(HTML('<style>div.prompt {display:none}</style>'))\n",
  		  "display(HTML('<style>div.input{display:none;}</style>'))"
 		  ]
