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
<table>  <tr><th><div style="width:290px">Scratch&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</div></th><th>Python</th></tr>
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
 <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/bounce.png" /></td>
      <td>
<pre lang="python">
cat.bounce_if_on_edge(10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_rotation_style.png" /></td>
      <td>
<pre lang="python">
cat.set_rotation_style(sg.RotationStyles.LEFT_RIGHT)
cat.set_rotation_style(sg.RotationStyles.DONT_ROTATE)
cat.set_rotation_style(sg.RotationStyles.ALL_AROUND)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/position_xy_dir.png" /></td>
      <td>
<pre lang="python">
a = cat.x
b = cat.y
c = cat.direction
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/say_for.png" /></td>
      <td>
<pre lang="python">
cat.say("Hello!")
game.wait(2)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/say.png" /></td>
      <td>
<pre lang="python">
cat.say("Hello!")
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/switch_costume.png" /></td>
      <td>
<pre lang="python">
cat.set_costume(1)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/next_costume.png" /></td>
      <td>
<pre lang="python">
cat.next_costume()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/switch_backdrop.png" /></td>
      <td>
<pre lang="python">
game.set_backdrop_idx(1)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/next_backdrop.png" /></td>
      <td>
<pre lang="python">
game.next_backdrop()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/change_size.png" /></td>
      <td>
<pre lang="python">
cat.change_size(10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_size.png" /></td>
      <td>
<pre lang="python">
cat.set_size(100)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/show.png" /></td>
      <td>
<pre lang="python">
cat.show()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/hide.png" /></td>
      <td>
<pre lang="python">
cat.hide()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/z_index.png" /></td>
      <td>
<pre lang="python">
cat.go_forward()
cat.go_backward()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/play_until.png" /></td>
      <td>
<pre lang="python">
cat.play_sound_until_done('C:\\Path\\meow.wav')
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/start_sound.png" /></td>
      <td>
<pre lang="python">
cat.play_sound('C:\\Path\\meow.wav')
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/change_volume.png" /></td>
      <td>
<pre lang="python">
cat.change_volume(-10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_volume.png" /></td>
      <td>
<pre lang="python">
cat.set_volume(100)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/get_volume.png" /></td>
      <td>
<pre lang="python">
a = cat.volume
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/start.png" /></td>
      <td>
<pre lang="python">
def cat_start(self: sg.Sprite):
    #...    
cat.add_event(sg.Events.START, cat_start)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/key.png" /></td>
      <td>
<pre lang="python">
def my_func(self: sg.Sprite):
    #...
cat.add_event(sg.Events.SPACE, my_func)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/sprite_clicked.png" /></td>
      <td>
<pre lang="python">
def my_func(self: sg.Sprite):
    #...
cat.add_event(sg.Events.MOUSE_LEFT, my_func)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/backdrop_switches.png" /></td>
      <td>
<pre lang="python">
def my_func(self: sg.Sprite):
    #...
cat.add_event(sg.Events.BACKDROP_SWITCHES_TO, my_func, 1)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/receive_message.png" /></td>
      <td>
<pre lang="python">
def my_func(self: sg.Sprite):
    #...
cat.add_event(sg.Events.RECEIVE_MESSAGE, my_func, "my_msg")
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/broadcast_message.png" /></td>
      <td>
<pre lang="python">
cat.broadcast_message("my_msg")
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/wait.png" /></td>
      <td>
<pre lang="python">
game.wait(1)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/repeat.png" /></td>
      <td>
<pre lang="python">
for i in range(10):
    #...
    game.wait(0.03)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/forever.png" /></td>
      <td>
<pre lang="python">
while True:
    #...
    game.wait(0.03)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/if.png" /></td>
      <td>
<pre lang="python">
if a == 50:
    #...
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/if_else.png" /></td>
      <td>
<pre lang="python">
if a == 50:
    #...
else:
    #...
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/wait_until.png" /></td>
      <td>
<pre lang="python">
while a != 50:
    game.wait(0.03)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/repeat_until.png" /></td>
      <td>
<pre lang="python">
while a != 50:
    #...
    game.wait(0.03)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/stop_all.png" /></td>
      <td>
<pre lang="python">
game.stop_all()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/start_as_clone.png" /></td>
      <td>
<pre lang="python">
def my_func(self: sg.Sprite):
    #...
clone.add_event(sg.Events.START, my_func)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/create_clone.png" /></td>
      <td>
<pre lang="python">
clone = cat.clone()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/delete_clone.png" /></td>
      <td>
<pre lang="python">
clone.delete()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/touching_mouse.png" /></td>
      <td>
<pre lang="python">
cat.is_touching_mouse()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/touching_edge.png" /></td>
      <td>
<pre lang="python">
cat.is_touching_edge()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/touching_sprite.png" /></td>
      <td>
<pre lang="python">
cat.is_touching_sprite(sprite)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/touching_color.png" /></td>
      <td>
<pre lang="python">
cat.is_touching_color((0, 0, 0))
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/color_touching_color.png" /></td>
      <td>
<pre lang="python">
game.are_colors_touching((0, 0, 0), (255, 255, 255))
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/distance_to_mouse.png" /></td>
      <td>
<pre lang="python">
cat.get_distance_to_mouse()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/distance_to_sprite.png" /></td>
      <td>
<pre lang="python">
cat.get_distance_to_sprite(sprite)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/ask.png" /></td>
      <td>
<pre lang="python">
a = cat.ask("What's your name?")
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/key_pressed.png" /></td>
      <td>
<pre lang="python">
game.is_key_pressed(sg.Keys.SPACE)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/mouse_down.png" /></td>
      <td>
<pre lang="python">
game.is_mouse_down
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/mouse_x.png" /></td>
      <td>
<pre lang="python">
game.mouse_x
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/mouse_y.png" /></td>
      <td>
<pre lang="python">
game.mouse_y
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_drag_mode.png" /></td>
      <td>
<pre lang="python">
cat.is_draggable = True
cat.is_draggable = False
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/timer.png" /></td>
      <td>
<pre lang="python">
game.timer()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/reset_timer.png" /></td>
      <td>
<pre lang="python">
game.reset_timer()
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/backdrop_of.png" /></td>
      <td>
<pre lang="python">
game.current_backdrop_idx
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/x_position_of.png" /></td>
      <td>
<pre lang="python">
cat.x
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/current_year.png" /></td>
      <td>
<pre lang="python">
import datetime
today = datetime.date.today()
year = today.year
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/days_since.png" /></td>
      <td>
<pre lang="python">
from datetime import date
today = date.today()
d = date(2000, 1, 1)
delta = today - d
print(delta.days)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/plus.png" /></td>
      <td>
<pre lang="python">
a + 2
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/minus.png" /></td>
      <td>
<pre lang="python">
a - 2
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/mul.png" /></td>
      <td>
<pre lang="python">
a * 2
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/div.png" /></td>
      <td>
<pre lang="python">
a / 2
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/random.png" /></td>
      <td>
<pre lang="python">
import random
random.randint(1, 10)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/greater.png" /></td>
      <td>
<pre lang="python">
a > 50
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/lower.png" /></td>
      <td>
<pre lang="python">
a < 50
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/equals.png" /></td>
      <td>
<pre lang="python">
a == 50
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/and.png" /></td>
      <td>
<pre lang="python">
a > 1 and b > 1
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/or.png" /></td>
      <td>
<pre lang="python">
a > 1 or b > 1
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/not.png" /></td>
      <td>
<pre lang="python">
not a > 1 
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/join.png" /></td>
      <td>
<pre lang="python">
"apple" + "banana"
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/letter_of.png" /></td>
      <td>
<pre lang="python">
"apple"[0]
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/length_of.png" /></td>
      <td>
<pre lang="python">
len("apple")
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/contains.png" /></td>
      <td>
<pre lang="python">
"a" in "apple"
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/mod.png" /></td>
      <td>
<pre lang="python">
a % 2
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/round.png" /></td>
      <td>
<pre lang="python">
round(a)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/abs.png" /></td>
      <td>
<pre lang="python">
abs(a)
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/set_var.png" /></td>
      <td>
<pre lang="python">
a = 0
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/change_var.png" /></td>
      <td>
<pre lang="python">
a += 1
</pre> 
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/def.png" /></td>
      <td>
<pre lang="python">
def my_block(steps):
    cat.move(steps)
</pre> 
      </td>
  </tr>
    <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/my_block.png" /></td>
      <td>
<pre lang="python">
my_block(10)
</pre> 
      </td>
  </tr>
</table>

