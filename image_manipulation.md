## recursive svg to png 
brew install librsvg
for i in *; do rsvg-convert --width=512 --height=512 $i -o `echo $i | sed -e 's/svg$/png/'`; done
