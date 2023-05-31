From Bhante Sujato:

I used the fonts downloaded from Google Fonts as listed in the Thai National Fonts. (Sarabun is already installed on Ubuntu, but the results were different, so there is a difference in the font or its handling. There were certain bugs in the pre-installed version that are absent in the Google Fonts one.)

I tried using the thaispec package (see my first draft to Dheerayupa). It seems the purpose of that is to use Thai characters mixed with Roman, in which case it would be great. But by itself, it seems to override any other font choices, so to use different fonts I abandoned that. Instead use Polyglossia for Thai support.

Swath did the preprocessing, it can be installed on Ubuntu with 
sudo apt install swath

Run Swath with 
swath -f latex -u u,u < input.tex > output.tex