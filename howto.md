* g o a t s e x * g o a t s e x * g o a t s e x * g o *
g                                                     g 
o /     \             \                  /    \       o
a|       |             \                |      |      a
t|       `.             |               |       :     t
s`        |             |              \|       |     s
e \       | /       /  \\\   --________ \\       :    e
x  \      \/   _--~~          ~--________| \     |    x 
*   \      \_-~                    ~-_______\    |    *
g    \_     \        _.--------.____________\|   |    g
o      \     \______// _ ___ _______ (_(__>  \   |    o
a       \   .  C ___)  ____________ (_(____>  |  /    a
t       /\ |   C ____)/            \ (_____>  |_/     t
s      / /\|   C_____) hello user   | (___>   /  \    s
e     |   (   _C_____) welcome from | // _/ /     \   e
x     |    \  |__   \\______________/// (__/       |  x
*    | \    \____)   `----   --------'             |  *
g    |  \_          ___\       /_______          _/ | g
o   |              /    |     |        \            | o
a   |             |    /       \        \           | a
t   |          / /    |         |        \           |t
s   |         / /      \__/\___/          |          |s
e  |           /        |    |             |         |e
x  |          |         |    |             |         |x
* g o a t s e x * g o a t s e x * g o a t s e x * g o *


create new image
(render lines into block line by line)
and then fit the line width by shifting and duplicating 
horizontal lines in right part of image


we should have some 2d matrix in which we'll store 
the rendered image
we should render text and then impose some immutable parts
of original image to it as a frame:

top part of frame


* g o a t s e x * g o a t s e x * g o a t s e x *
g                                               g 
o /     \             \            /    \       o
a|       |             \          |      |      a
t|       `.             |         |       :     t
s`        |             |        \|       |     s
e \       | /       /  \\\   --__ \\       :    e
x  \      \/   _--~~          ~--__| \     |    x 
*   \      \_-~                    ~-_\    |    *
g    \_     \        _.--------.______\|   |    g
o      \     \______// _ ___ _ (_(__>  \   |    o
a       \   .  C ___)  ______ (_(____>  |  /    a
t       /\ |   C ____)/      \ (_____>  |_/     t


bottom part of frame


e     |   (   _C_____)\______/  // _/ /     \   e
x     |    \  |__   \\_________// (__/       |  x
*    | \    \____)   `----   --'             |  *
g    |  \_          ___\       /_          _/ | g
o   |              /    |     |  \            | o
a   |             |    /       \  \           | a
t   |          / /    |         |  \           |t
s   |         / /      \__/\___/    |          |s
e  |           /        |    |       |         |e
x  |          |         |    |       |         |x
* g o a t s e x * g o a t s e x * g o a t s e x *


left center part of frame


g    \_     \        _.-
o      \     \______// _
a       \   .  C ___)  _
t       /\ |   C ____)/ 
s      / /\|   C_____) 
e     |   (   _C_____)\_
x     |    \  |__   \\__
*    | \    \____)   `--
g    |  \_          ___\
o   |              /    
a   |             |    /
t   |          / /    | 
s   |         / /      \
e  |           /        
x  |          |         
* g o a t s e x * g o a 


right center part of frame 


  ~--__| \     |    x  
       ~-_\    |    *
---.______\|   |    g
 _ (_(__>  \   |    o
_ (_(____>  |  /    a
 \ (_____>  |_/     t
 |  (___>   /  \    s
_/  // _/ /     \   e
___// (__/       |  x
 --'             |  *
   /_          _/ | g
  |  \            | o


we need to find optiomal subpatterns in which we can place
any text parts


