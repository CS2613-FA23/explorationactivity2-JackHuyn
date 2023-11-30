## Package/ Library Overview
#### Which package/library did you select?
I select the pygame package in python to be my 2nd topic research, i also working with Namneet for the EA2, we both code and tryout pygame and pandas at the same time.

1.  What is the package/library?

        What purpose does it serve?

            The pandas library in python is used for analyzing, cleaning, exploring and manipulating data. So it mainly working with data sets. This library will be helpful for student that chosing Data Science as their major.

            The pygame is used to create some game by using images, the program will display multiple image per second on the screen. 

2.  How do you use it?

        You can just simply import the pandas/pygame from the library after install it.

    To install it?

        If you are using Visual Studio Code, open your terminal then simply type in "pip install pandas" . This will install every package you need to use pandas in python

        If you are using Mac, you have to ensure that you have python3 and pip3 up to date. You can check that by using:
        > python3 --version
        > pip3 --version

        If you want to make sure that your pip3 version run perfectlym you can update it by:
        > pip3 install --upgrade pip
    
        To install pandas, type : > "pip3 install pandas" in the terminal. 
        To install pygame, type : > "pip3 install pygame"
    
    Function used when using pandas

    Dataframe()

            This function convert a array of data into a Dataframe ( use for multitple data input)

            Ex: data = pandas.DataFrame(sth)

    Basic function for pygame

    pygame.init()

            This line here need to run everytime in the main program, this will initial all the need function for the game

    screen = pygame.display.set_mode(width, height) 

            this line will create a black screen with the dimension specify by the user and call it screen
    
    clock = pygame.time.Clock()
    clock.tick(60)

            Here you create a clock class, then set the tick to 60
            which can be understand as there will be no more than 60 image being display per sec 

            This line of code is importand since it determine how fast your game will be

            On the other hand, this can be also understand as FPS (Frame per second)

    pygame.display.update()

            The main code will need to be updated per clock tick
            this will display all the images per tick

    pygame.display.set_caption("Tetris")

            This will set your window title as "Tetris" you can modify the string inside the ""


    Creating surface/area and display a images

            Everytimg you want to display an image into your screen 
            you want to create a surface and then display that on your surface

            Ex:
            color_surf = pygame.Surface((100,200))
            color_surf.fill('Red')

            # this 2 lines of code will create a surface that have a size of 100x200, then fill the surface with the color red

        
    Example block of code

            while True:
                #checks if "quit" is in the list of events and exits if true
                for event in pygame.event.get():
                    if event.type == pygame.QUIT:
                        pygame.quit()
                        sys.exit()
                    if event.type == pygame.KEYDOWN:
                        print('Down')

            In this example, if you want to let the code keep running, you can use the while true, or can specify the condition for when the game should run

            when the program is running, pygame has lots of events happen per frame, so the pygame.event.get() will return a list of event
            the event.type will return the type of that event.

            You can explore more about the event type in pygame doc (1)

    Display image on top of each other

            you can achhive this using blit (stand for block image transfer aka (regular) surface on another surface)

            ex:
                Let take the screen and the color_surf above

                screen.blit(color_surf, (x,y))

                here x and y are the position to place them, it always be the top-left corner of the color surface


    If you loading the image from the file, you can simply do this:

            player_stand = pygame.image.load('graphics/player/player_stand.png').convert_alpha()

            play_stand_rect = player_stand.get_rect(center = (400,200))

            screen.blit(player_stand, player_stand_rect)

            This will place the player image within the player_rect at location 400x200, the get_rect will return the dimension of the image, create a surface for it


        
        
3.  What are the functionalities of the package?/library?

    Pandas
    a  To analyze the data set from JSON, csv or excel file. 
    b  To make a graph, calculate probability, vv
    c  Mainly for working with data sets

    Pygame
    To display image, play sound 
    It also can handle colission between images vs images (ex: hitbox, boundary, etc..)

4.  When was it created?

    Pandas was created in January 11 2008
    Pygame was created in October 28 2000 (2)

5.  Why did you select this package/library?

    I choose pandas as my topic research because my major is Data Science, this will be my foundation for me future project as well as improve my knowledge when handling data sets problem.

    I choose the pyagme for the second exploration because around the middle of the term, i found my interest in trying new stuff and i think of working on a simple game.

6.  How did learning the package/library influence your learning of the language?

    Exporing pandas help me to understand more about python, it was really fun to study this and manipulate data set that i found.

    Learning pygame take more time than expected, but it help a lot when it coming to working with OOP classes.


7.  How was your overall experiences with the package/library?

    From a scale from 1-10, I'm thinking that I'm around 6-7 at the moment, i need more practice as well as some experiences to manipulate/ understand more function

    It was really fun when coding the game, lots of mistake, but i learn more from failing. 

## References
(1) https://en.wikipedia.org/wiki/Pygame

(2) https://www.pygame.org/docs/

