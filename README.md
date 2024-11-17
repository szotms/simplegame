# simplegame
Python package for creating simple games.
# installation
```
pip install simplegame
```
# quick start
```python
from simplegame import sg

def cat_start(self: sg.Sprite):
    for x in range(30):
        self.move(10)
        game.wait(0.03)

game = sg.Game(900, 500)

cat = game.create_sprite(150, 250, ['C:\\Path\\cat.png'])
cat.add_event(sg.Events.START, cat_start)

game.run()
```
# scratch - python comparision
<img src="https://github.com/szotms/simplegame/blob/main/images/quick_start2.png" />
<table>
  <tr><th>Scratch</th><th>Python</th></tr>
  <tr><td><img src="https://github.com/szotms/simplegame/blob/main/images/scratch_coords.png" /></td>
        <td><img src="https://github.com/szotms/simplegame/blob/main/images/python_coords.png" /></td></tr>
    <tr><td><img src="https://github.com/szotms/simplegame/blob/main/images/scratch_dir.png" /></td>
        <td><img src="https://github.com/szotms/simplegame/blob/main/images/python_dir.png" /></td></tr>
  <tr><td><img src="https://github.com/szotms/simplegame/blob/main/images/quick_start.png" /></td><td>
    
```python
import simplegame as sg

def cat_start(self: sg.Sprite):
    while True:
        self.move(10)
        game.wait(0.2)

game = sg.Game(900, 500)

cat = game.create_sprite(150, 250, ['C:\\Path\\cat.png'])
cat.add_event(sg.Events.START, cat_start)

game.run()
```

  </td></tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/move.png" /></td>
      <td>
<pre lang="python">
cat.move(10)
</pre>
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/turn_right.png" /></td>
      <td>
<pre lang="python">
cat.change_direction(15)
</pre>   
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/turn_left.png" /></td>
      <td>
<pre lang="python">
cat.change_direction(-15)
</pre>   
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/go_to_random.png" /></td>
      <td>
<pre lang="python">
cat.go_to_random()
</pre> 
      </td>
  </tr>
 <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/go_to_mouse.png" /></td>
      <td>
<pre lang="python">
cat.go_to_mouse()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/go_to_sprite.png" /></td>
      <td>
<pre lang="python">
cat.go_to_sprite(sprite)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/go_to_xy.png" /></td>
      <td>
<pre lang="python">
cat.set_x(0)
cat.set_y(0)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/glide_to_random.png" /></td>
      <td>
<pre lang="python">
x = random.randint(0, game.width)
y = random.randint(0, game.height)
cat.glide_to(1, x, y)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/glide_to_mouse.png" /></td>
      <td>
<pre lang="python">
x = game.mouse_x
y = game.mouse_y
cat.glide_to(1, x, y)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/glide_to_sprite.png" /></td>
      <td>
<pre lang="python">
x = sprite.x
y = sprite.y
cat.glide_to(1, x, y)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/glide_to_xy.png" /></td>
      <td>
<pre lang="python">
cat.glide_to(1, 0, 0)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/point_in_direction.png" /></td>
      <td>
<pre lang="python">
cat.set_direction(90)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/point_towards_mouse.png" /></td>
      <td>
<pre lang="python">
x = game.mouse_x
y = game.mouse_y
cat.set_direction_to_xy(x, y)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/point_towards_sprite.png" /></td>
      <td>
<pre lang="python">
x = sprite.x
y = sprite.y
cat.set_direction_to_xy(x, y)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/change_x.png" /></td>
      <td>
<pre lang="python">
cat.change_x(10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_x.png" /></td>
      <td>
<pre lang="python">
cat.set_x(0)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/change_y.png" /></td>
      <td>
<pre lang="python">
cat.change_y(10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_y.png" /></td>
      <td>
<pre lang="python">
cat.set_y(0)
</pre> 
      </td>
  </tr>

</table>

