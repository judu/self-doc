# How to have operator mono lig with bold on my computer


- Purchase the Operator Mono SSm font
- Go to https://github.com/kiliman/operator-mono-lig and follow the instructions

**Issue:** the otf files define weird weight. That makes fontconfig choose the bold _files_ for non bold fonts…


To fix that, I put together the 90-operator-weight.conf file to put to
`~/.config/fontconfig/conf.d/`.
The current file works :shrug:.
