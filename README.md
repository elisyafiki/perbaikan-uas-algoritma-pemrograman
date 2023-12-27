# perbaikan-uas-algoritma-pemrograman
def turn_right():
    turn_left()
    turn_left()
    turn_left()
    
def turn_180():
    turn_left()
    turn_left()
    
while not at_goal(): move()
turn_right();
while not wall_in_front(): move();
turn_left()

def handle_possible_wall():
    move()
    wr = wall_on_right()
    turn_180()
    move()
    turn_left()
    if wr:
        build_wall()
        turn_left()
    else:
        move()
        
while not at_goal():
    if right_is_clear():
        handle_possible_wall()
    elif front_is_clear():
        move();
    else: 
        turn_left()
