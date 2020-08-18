# sleep-until-modified

A bash script to be used as the condition in a while-loop in order to perform a command when a file is changed.

For example, the below code runs `pdflatex` whenever the user saves a given LaTeX file.

```
TEX=report.tex
while sleep-until-modified $TEX ;
do
	pdflatex $TEX;
done
```

Make sure to give the script execution permission with `chmod +x`. Stop the script with `Ctrl+C`.
