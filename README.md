# AHPtableGenerator
Simple interactive Python script that generates a Analitic Hierarchy Process table, it exports a fully editable .tex code file and a .pdf file.

## Requirements

1. LaTeX installed<br/>

		sudo apt-get install texlive-full
2. Python >= 3.6 installed<br/>
		
		python3 -V
3. numpy package<br/>

		pip3 install numpy
4. PyLaTeX package<br/>

		pip3 install pylatex

### For the venv enjoyers
1. Move to your venv folder<br/>

		cd ~/.venv
2. Create the venv<br/>

		python3 -m venv PyLaTeXvenv
3. Activate the virtual enviroment<br/>

		source PyLaTeXvenv/bin/activate
4. Install the required packages<br/>

		pip install -r requirements.txt
5. View the installed packages<br/>

		pip3 list

## Installation

	git clone https://github.com/hasecilu/AHPtableGenerator.git

## Usage in terminal
1. Open the folder via terminal<br/>

		cd AHPtableGenerator
2. Run the script via terminal<br/>

		python3 AHPtableGenerator.py
or<br/>

	source ~/.venvs/PyLaTeXvenv/bin/activate
	python3 AHPtableGenerator.py

3. Follow the instructions in the terminal
4. Open the .pdf file<br/>

		xdg-open filename.pdf
5. View the .tex file<br/>

		less filename.tex
6. Modify the .tex file if needed it and add it to your document

## Example of generated file

### Code
Small portion of generated code (indentation not included).

```latex
\usepackage{booktabs} % Add this line to the preamble (before \begin{document})
...
\begin{table}[!ht]
	\centering
	\begin{tabular}{ccccccc}
		\toprule
		Criterios &   R    &   G    &   B    &   W    & Total de fila & Vector de prioridad \\ \midrule
		    R     & 0.0769 & 0.0345 & 0.1053 & 0.0704 &    0.2871     &    {[}0.0718{]}     \\
		    G     & 0.1538 & 0.069  & 0.0526 & 0.0845 &    0.3599     &     {[}0.09{]}      \\
		    B     & 0.3077 & 0.5517 & 0.4211 & 0.4225 &     1.703     &    {[}0.4258{]}     \\
		    W     & 0.4615 & 0.3448 & 0.4211 & 0.4225 &    1.6499     &    {[}0.4125{]}     \\ \midrule
		  Suma    & 0.9999 &  1.0   & 1.0001 & 0.9999 &    3.9999     &    {[}1.0001{]}     \\ \bottomrule
	\end{tabular}
	\caption{Table caption}
\end{table}
```
### pdf file
![Example](https://raw.github.com/hasecilu/AHPtableGenerator/master/images/example2.png)

