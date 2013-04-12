Werewolves
==========

The game
--------

The game follows a night and day cycle. 
* At night, the werewolf picks a villager to kill, while everyone else "sleeps". 
* During the day, the villagers wake up and discover that one of them has died, so they will discuss who might be the werewolf. The villagers lynch their guess, hoping it's the wolf. The villagers win if they kill the werewolf; the werewolf wins if there is only one villager left.

The following roles can be distinguished:
* Villager – The villager is the simplest role. In the daytime, you vote on who to kill. You try to narrow down who the wolf is. 
* Werewolf – The wolf kills one of the villagers during the night. During the day, the werewolf acts a villager trying to avoid suspicion. 


Starting a game
---------------

* To start a game, you need to send the following chatmessage to the Game Coordinator (Jabber Id "sww@jabber.org" or "sww@localserver"). The Game Coordinator will react by dispatching you to a chatroom.

        I want to play 
    

* To indicate you are a candidate to play the werewolf role, send the following _private_ chatmessage to the Master of Ceremonies of the chatroom (Jabber Id "softwarewolf"). Any string containing werewolf will work. The MC will only take into account requests until the game starts.

        werewolf
        
* Upon start of the game, the MC notifies the player that is elected as werewolf by replying:

        You are selected as werewolf for this game. 
  
Commands for playing the game
-----------------------------

* During the night, the werewolf can use send the following _private_ message to the MC to choose which player to eat:

        I eat <playername>
        
* During the day, a villager can cast a vote to hang the player suspected of being a werewolf by sending the following chatroom message. The player with the majority vote will be lynched. 

        I vote for <playername> 

Interpreting the game progress
------------------------------

The MC outputs information as the game progresses.

###Switching between night and day

Night and day last for a particular time period. To inform all players when the switch between night and day occurs, the MC changes the chatroom subject accordingly:
* The chatroom topic that indicates it's the werewolves turn:

        Night
        
* The chatroom topic that indicates it's the villagers turn:

        Day


###Private messages from the MC to the werewolf
* At the start of each night, the MC indicates it is time for the werewolf to select a victim by sending the following private message to the werewolf:

        Please choose who you want to eat: <playername1>,<playername2>,…,<playernameN>

###Chatroom messages (visible to all players)
* At the start of each day, the MC informs all players which player was killed by of the werewolf last night by posting the following message in the chatroom:

        The werewolf ate <Playername>
        
* Subsequently, the MC invites all players to vote who should be hanged by posting the following message:

        Please vote who should be hanged: <playername1>,<playername2>,…,<playernameN>
        
* After all votes have been cast (or the time for voting expires), the MC counts the votes and posts the following message to inform all players who was hanged:

        The villagers hanged <Playername>
        
* In case the villagers hanged the werewolf, the MC posts the following message to inform the villagers they have won the game:

        Yes! The last werewolve is dead! Finally peace in the village! The villagers win.
        
* In case there is only one villager left next to the werewolf, the MC posts the following message to inform all players the werewolf has won the game:

        Oh no! Villagers do not outnumber werewolves anymore, so the werewolves know they are stronger and mount a daytime massacre and slaughter all remaining villagers! - The werewolves win.


