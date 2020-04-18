# Nathaniel Maxwell
# Integration Project
# Sports Extravaganza

points_1 = 0 # easy
points_2 = 0 # meduim
points_3 = 0 # hard
points_4 = 0 # legend
restarts = 0 # restarts
x = 0 # main menu
y = 0 # credits
w = 0 # leaderboard
a = 0 # easy
b = 0 # medium
c = 0 # hard
d = 0 # legend
while x < 1:
    print("1:Start Quiz")
    print("2:Cerdits")
    print("3:Leaderboards")
    print("4:Exit")
    main_menu = int(input("What would you like to do? "))
    if main_menu == 1:
        name = input("Welcome! What is your name? ")
        print(("I hope you enjoy the Sports Extravaganza "), name, ("!"), sep = "")
        print("Here we go")
        x = 2
    elif main_menu == 2:
        while y < 1:
            print("Questions by Nathan Maxwell")
            print("Made by Nathan Maxwell")
            print("Are you done?")
            in_credit = int(input("1: yes or 2: no "))
            if in_credit == 1:
                y = 2
                x = 0
            else:
                y = 0
                x = 2
    elif main_menu == 3:
        def main():
            leaderboard_list = open('leaderboard.txt')
            lb = leaderboard_list.read()
            print(lb)
        main()
    elif main_menu == 4:
        print("I hope you enjoyed the Sports Extravaganza!")
        x = 2

# Every question right get 1 pts
# Every question wrong -1 pts and reset
# Checkpoint every 5 questions
# Gets harder as goes on
# POGIL to find what to use and exercises
while a < 1:
    print("Question #1")
    print("Who won the Super Bowl in the 2019-2020 NFL season?")
    print("1:New England Patriots")
    print("2:Kansas City Cheifs")
    print("3:San Fransico 49ers")
    print("4:Green Bay Packers")
    answer_1 = int(input())
    if answer_1 == 1:
        print("You're a year behind")
        points_1 -= 1
    elif answer_1 == 2:
        print("Glad to see you watched the Super Bowl")
        points_1 += 1
    elif answer_1 == 3:
        print("They kinda blew it")
        points_1 -= 1
    elif answer_1 == 4:
        print("No chance at all")
        points_1 -= 1
    print(("You now have: "), points_1, (" point(s)"), sep="")

    print("Question #2")
    print("What NFL team has the most Super Bowl wins?")
    print("1:Pittsburgh Steelers")
    print("2:Dallas Cowboys")
    print("3:San Fransico 49ers")
    print("4:New England Patriots")
    answer_2 = int(input())
    if answer_2 == 1:
        print("You got it")
        points_1 += 1
    elif answer_2 == 2:
        print("Cowboy fans wish")
        points_1 -= 1
    elif answer_2 == 3:
        print("Close but no cigar")
        points_1 -= 1
    elif answer_2 == 4:
        print("Did two right answers trip you up")
        points_1 += 1
    print(("You now have: "), points_1, ( "point(s)"), sep="")

    print("Question #3")
    print("What player in the NBA is known as the Black Mamba")
    print("1:LeBron James")
    print("2:Kobe Bryant")
    print("3:Micheal Jordan")
    print("4:Larry Bird")
    answer_3 = int(input())
    if answer_3 == 1:
        print("Thats King James")
        points_1 -= 1
    elif answer_3 == 2:
        print("What happened is truly sad. Have two points to honor him and Gigi")
        points_1 += 2
    elif answer_3 == 3:
        print("He's the GOAT")
        points_1 -= 1
    elif answer_3 == 4:
        print("Larry Legend")
        points_1 -= 1
    print(("You now have: "), points_1, ( "point(s)"), sep="")

    print("Question #4")
    print("What brand makes NBA jerseys?")
    print("1:Adidas")
    print("2:Under Armour")
    print("3:Nike")
    print("4:Jordan")
    answer_4 = int(input())
    if answer_4 == 1:
        print("Wrong sport")
        points_1 -= 1
    elif answer_4 == 2:
        print("Too small")
        points_1 -= 1
    elif answer_4 == 3:
        print("They are everywhere anymore")
        points_1 += 1
    elif answer_4 == 4:
        print("They just do shoes")
        points_1 -= 1
    print(("You now have: "), points_1, ( "point(s)"), sep="")

    print("Question #5")
    print("What player plays for Argentina in the Mens World Cup?")
    print("1:Cristiano Ronaldo")
    print("2:Neymar Jr")
    print("3:Harry Kane")
    print("4:Lionel Messi")
    answer_5 = int(input())
    if answer_5 == 1:
        print("Plays for Portugal")
        points_1 -= 1
    elif answer_5 == 2:
        print("Plays for Brazil")
        points_1 -= 1
    elif answer_5 == 3:
        print("Plays for England")
        points_1 -= 1
    elif answer_5 == 4:
        print("What a Legend of the sport")
        points_1 += 1
    print(("You now have: "), points_1, ( "point(s)"), sep="")

    print("I'm glad to see you made it past the very easy section.")
    print("Lets see how you're doing.")
    if points_1 >= 4:
        print("You made it past the easy section!")
        a = 2
    else:
        print("You failed the easy section and have to redo.")
        a = 0
        points_1 = 0
        restarts += 1

while b < 1:
    print("Question #6")
    print("How many strikes do you have to get in order to bowl a 300?")
    print("1:11")
    print("2:12")
    print("3:10")
    print("4:13")
    answer_6 = int(input())
    if answer_6 == 1:
        print("that's a 290 game")
        points_2 -= 1
    elif answer_6 == 2:
        print("300!")
        points_2 += 1
    elif answer_6 == 3:
        print("Your a few off")
        points_2 -= 1
    elif answer_6 == 4:
        print("There is not 13 frames")
        points -= 1
    print(("You now have: "), points_2, ( "point(s)"), sep="")

    print("Question #7")
    print("How many superbowls have there been in NFL history?")
    print("1:50")
    print("2:52")
    print("3:54")
    print("4:56")
    answer_7 = int(input())
    if answer_7 == 1:
        print("That was in 2016")
        points_2 -= 1
    elif answer_7 == 2:
        print("That was in 2018")
        points_2 -= 1
    elif answer_7 == 3:
        print("It's been 54 years strong")
        points_2 += 1
    elif answer_7 == 4:
        print("That will be in 2022")
        points_2 -= 1
    print(("You now have: "), points_2, ( "point(s)"), sep="")

    print("Question #8")
    print("How many teams are there in the WNBA?")
    print("1:12")
    print("2:13")
    print("3:10")
    print("4:11")
    answer_8 = int(input())
    if answer_8 == 1:
        print("There are only 12 teams")
        points_2 += 1
    elif answer_8 == 2:
        print("That's to many teams")
        points_2 -= 1
    elif answer_8 == 3:
        print("They have more than 10")
        points_2 -= 1
    elif answer_8 == 4:
        print("You're just off")
        points_2 -= 1
    print(("You now have: "), points_2, ( "point(s)"), sep="")

    print("Question #9")
    print("Who was the finals MVP in 2015?")
    print("1:Klay Thompson")
    print("2:Steph Curry")
    print("3:Kevin Durant")
    print("4:Andre Iguodala")
    answer_9 = int(input())
    if answer_9 == 1:
        print("He has yet to get one")
        points_2 -= 1
    elif answer_9 == 2:
        print("Regulare season MVP, but not finals")
        points_2 -= 1
    elif answer_9 == 3:
        print("He was not there yet")
        points_2 -= 1
    elif answer_9 == 4:
        print("For his defense on LeBron")
        points_2 += 1
    print(("You now have: "), points_2, ( "point(s)"), sep="")

    print("Question #10")
    print("When was the last time the lions made the playoffs?")
    print("1:1992")
    print("2:2016")
    print("3:2017")
    print("4:2008")
    answer_10 = int(input())
    if answer_10 == 1:
        print("That was their last won")
        points_2 -= 1
    elif answer_10 == 2:
        print("It was pretty recent")
        points_2 += 1
    elif answer_10 == 3:
        print("They went 9-7 and missed")
        points_2 -= 1
    elif answer_10 == 4:
        print("They went 0-16...")
        points_2 -= 1
    print(("You now have: "), points_2, ( "point(s)"), sep="")

    print("I'm glad to see you made it past the medium section.")
    print("Lets see how you're doing.")
    if points_2 >= 3:
        print("You made it past the medium section!")
        b = 2
    else:
        print("You failed the meduim section and have to redo.")
        b = 0
        points_2 = 0
        restarts += 1

while c < 1:
    print("Question #11")
    print("What is the record for most points scored in an NBA playoff game?")
    print("1:68")
    print("2:81")
    print("3:70")
    print("4:100")
    answer_11 = int(input())
    if answer_11 == 1:
        print("Jordan drop 68 in a playoff game")
        points_3 += 1
    elif answer_11 == 2:
        print("Kobe did this in the regular season")
        points_3 -= 1
    elif answer_11 == 3:
        print("Booker did this in the regular season")
        points_3 -= 1
    elif answer_11 == 4:
        print("The regular season record")
        points_3 -= 1
    print(("You now have: "), points_3, ( "point(s)"), sep="")

    print("Question #12")
    print("Who writes 'I can do all things' on their shoes?")
    print("1:LeBron James")
    print("2:Steph Curry")
    print("3:Blake Griffin")
    print("4:Derrick Rose")
    answer_12 = int(input())
    if answer_12 == 1:
        print("He pays respect to players")
        points_3 -= 1
    elif answer_12 == 2:
        print("He does this")
        points_3 += 1
    elif answer_12 == 3:
        print("Does nothing")
        points_3 -= 1
    elif answer_12 == 4:
        print("He's just loved by the people")
        points_3 -= 1
    print(("You now have: "), points_3, ( "point(s)"), sep="")

    print("Question #13")
    print("What team was Derrick Rose on when he dropped his carrer high?")
    print("1:Chicago Bulls")
    print("2:Minnesota Timberwolves")
    print("3:Detroit Pistions")
    print("4:New York Knicks")
    answer_13 = int(input())
    if answer_13 == 1:
        print("Shockingly no")
        points_3 -= 1
    elif answer_13 == 2:
        print("When he dropped 50")
        points_3 += 1
    elif answer_13 == 3:
        print("His best efficiency")
        points_3 -= 1
    elif answer_13 == 4:
        print("He was just injured here")
        points_3 -= 1
    print(("You now have: "), points_3, ( "point(s)"), sep="")

    print("Question #14")
    print("How many Super Bowls have the Minnesota Vikings been too?")
    print("1:3")
    print("2:5")
    print("3:2")
    print("4:4")
    answer_14 = int(input())
    if answer_14 == 1:
        print("Close but they made more")
        points_3 = -1
    elif answer_14 == 2:
        print("That's to many for them")
        points_3 -= 1
    elif answer_14 == 3:
        print("That's half of them")
        points_3 -= 1
    elif answer_14 == 4:
        print("Been to 4 and won 0")
        points_3 += 1
    print(("You now have: "), points_3, ( "point(s)"), sep="")

    print("Question #15")
    print("How many people are on an NFL roster?")
    print("1:46")
    print("2:70")
    print("3:55")
    print("4:53")
    answer_15 = int(input())
    if answer_15 == 1:
        print("Players that suit up on game day")
        points_3 -= 1
    elif answer_15 == 2:
        print("Preseason roster size")
        points_3 -= 1
    elif answer_15 == 3:
        print("Thats the size after the CBA")
        points_3 += 1
    elif answer_15 == 4:
        print("That was last years roster size")
        points_3 -= 1
    print(("You now have: "), points_3, ( "point(s)"), sep="")

    print("I'm glad to see you made it past the hard section.")
    print("Lets see how you're doing.")
    if points_3 >= 3:
        print("You made it past the hard section!")
        c = 2
    else:
        print("You failed the hard section and have to redo.")
        c = 0
        points_3 = 0
        restarts += 1

while d < 1:
    print("Question #16")
    print("What year was Giannas Antetokounmpo drafted?")
    print("1:2012")
    print("2:2013")
    print("3:2014")
    print("4:2015")
    answer_16 = int(input())
    if answer_16 == 1:
        print("To early for him")
        points_4 -= 1
    elif answer_16 == 2:
        print("It's been 7 years now")
        points_4 += 1
    elif answer_16 == 3:
        print("Just missed his rookie season")
        points_4 -= 1
    elif answer_16 == 4:
        print("He's been in the league a few years")
        points_4 -= 1
    print(("You now have: "), points_4, ( "point(s)"), sep="")

    print("Question #17")
    print("How many grand slams have Serena Williams won?")
    print("1:20")
    print("2:27")
    print("3:23")
    print("4:7")
    answer_17 = int(input())
    if answer_17 == 1:
        print("Roger Federer has 20")
        points_4 -= 1
    elif answer_17 == 2:
        print("That's more than anyone has")
        points_4 -= 1
    elif answer_17 == 3:
        print("She is at 23")
        points_4 += 1
    elif answer_17 == 4:
        print("This is Venus Williams")
        points_4 -= 1
    print(("You now have: "), points_4, ( "point(s)"), sep="")

    print("Question #18")
    print("What's the most turnovers James Harden got in a single game?")
    print("1:13")
    print("2:12")
    print("3:11")
    print("4:14")
    answer_18 = int(input())
    if answer_18 == 1:
        print("He got 13 back in 2015")
        points_4 += 1
    elif answer_18 == 2:
        print("He did this in 2016 and still not his most")
        points_4 -= 1
    elif answer_18 == 3:
        print("He did this in 2020 but not his most")
        points_4 -= 1
    elif answer_18 == 4:
        print("He has not done this yet")
        points_4 -= 1
    print(("You now have: "), points_4, ( "point(s)"), sep="")

    print("Question #19")
    print("How mant championships does Jeff Gordon have?")
    print("1:2")
    print("2:5")
    print("3:3")
    print("4:4")
    answer_19 = int(input())
    if answer_19 == 1:
        print("That is to few for him")
        points_4 -= 1
    elif answer_19 == 2:
        print("Jimmy Johnson has 5")
        points_4 -= 1
    elif answer_19 == 3:
        print("Still to few for him")
        points_4 -= 1
    elif answer_19 == 4:
        print("He won 4 in his time")
        points_4 += 1
    print(("You now have: "), points_4, ( "point(s)"), sep="")

    print("Question #20")
    print("What team has gone to the most Super Bowls in NFL history?")
    print("1:Pittsburgh Steelers")
    print("2:Dallas Cowboys")
    print("3:New England Patriots")
    print("4:San Fransico 49ers")
    answer_20 = int(input())
    if answer_20 == 1:
        print("They only have been to 8")
        points_4 -= 1
    elif answer_20 == 2:
        print("Their fans wish")
        points_4 -= 1
    elif answer_20 == 3:
        print("They have been to 11")
        points_4 += 1
    elif answer_20 == 4:
        print("They have only been to 7")
        points_4 -= 1
    print(("You now have: "), points_4, ( "point(s)"), sep="")

    print("I'm glad to see you made it past the legend section.")
    print("Lets see how you're doing.")
    if points_4 >= 3:
        print("You made it past the legend section!")
        d = 2
    else:
        print("You failed the legend section and have to redo.")
        d = 0
        points_4 = 0
        restarts += 1

print("Congrats you made it to the end")
print("Let's see how you did")
points = (points_1 + points_2 + points_3 + points_4) #For leaderboard points
#End of the Quiz
def main():
    name = input("Name: ")
    print("Input the next two numbers you see on the screen.")
    points_lb = input(points)
    restarts_lb = input(restarts)
    in_file = open('leaderboard.txt', "a")
    in_file.write("\nName: " + name)
    in_file.write("\nPoints: " + points_lb)
    in_file.write("\nRestarts: " + restarts_lb)
    in_file.close()
main()

print("Would you like to see the leaderboard?")
print("1:yes")
print("2:no")
look_leaderboard = int(input())
if look_leaderboard == 1:
    while w < 1:
        def main():
            leaderboard_list = open('leaderboard.txt')
            lb = leaderboard_list.read()
            print(lb)
        main()
        print("Press 1 to exit")
        leave = int(input())
        if leave == 1:
            print("I hope you enjoyed the Sports Extravaganza.")
            print("See you next time!")
            w = 2
        else:
            w = 0
else:
    print("I hope you enjoyed the Sports Extravaganza.")
    print("See you next time!")
