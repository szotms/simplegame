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
    
```python
cat.move(10)
```

      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/turn_right.png" /></td>
      <td>

```python
cat.change_direction(15)
```
          
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/turn_left.png" /></td>
      <td>

```python
cat.change_direction(-15)
```
          
      </td>
  </tr>
  <tr>
      <td><img src="https://github.com/szotms/simplegame/blob/main/images/go_to_random.png" /></td>
      <td>

```python
cat.go_to_random()
```
          
      </td>
  </tr>
 

</table>

