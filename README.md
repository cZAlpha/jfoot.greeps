# G R E E P S   I N V A S I O N
![](./greeps-world.gif)
* **Purpose**
    * To establish familiarity with conditional statements
* **Objective**
    * Modify the `Greep` class to collect `Tomato` objects and return them to the `Spaceship` while avoiding `Water` and obstacles.
* **Description**
    * Your task is to program the `Greep` to collect as many `Tomato` as possible.
    * You may **ONLY CHANGE THE GREEP** class.
    * You may **not** change any other class.
* **Getting oriented**
    * Please view the [javadocs](https://curriculeon.github.io/jfoot.greeps/javadocs/index.html) for this project to get better acquainted with the object orientation
        * the [Creature](https://curriculeon.github.io/jfoot.greeps/javadocs/com/github/curriculeon/greeps/Creature.html) class is the abstract superclass of the `Greep` class.
        * the [Greep](https://curriculeon.github.io/jfoot.greeps/javadocs/com/github/curriculeon/greeps/Greep.html) is a concrete subclass of the `Creature` class.
        * the [GreepSpit](https://curriculeon.github.io/jfoot.greeps/javadocs/com/github/curriculeon/greeps/GreepSpit.html) is a _composite child_ of `Greep`. It is the permissible only communication mechanism by `Greep`s.
        * the [TomatoPile](https://curriculeon.github.io/jfoot.greeps/javadocs/com/github/curriculeon/greeps/TomatoPile.html) is where `Greep` gather resources. A `Greep` cannot retrieve from a `TomatoPile` unless another `Greep` is there to _load_ it onto the other `Greep` present at the same `TomatoPile`.

* **Development Constraints**  
    1. Only change the class `Greep`. No other classes may be modified or 
created.
    2. No additional fields. You cannot extend the `Greep` memory.
        * you are not allowed to add fields to the class (except final fields).
        * You can use the one byte memory that is provided.
    3. You cannot `move` more than once per `act` round.
    4. You cannot communicate directly with other `Greep`.
        * That is: no field accesses or method calls to other `Greep` objects are allowed.
        * `Greep` can communicate indirectly via the `GreepSpit` on the ground.
    5. No long vision.
        * You are allowed to look at the world only at the immediate location of the Greep.
        * `Greep` are almost blind, and cannot look any further.
    6. No instantiating `Actor` subclasses.
        * `Actor` subclasses, such as `Greep` or `GreepSpit`, cannot be instantiated. `Greep` have no magic powers - they cannot create things out of nothing.
    7. No teleporting.
        * Methods from `Actor` that cheat normal movement (such as `setLocation`) may not be used.
        
        
### Background
* This application is built using the [Jfoot](https://github.com/Git-Leon/jfoot-api) library.



<hr><hr>
## How to Download

#### Part 1 - Forking the Project
* To _fork_ the project, click the `Fork` button located at the top right of the project.


#### Part 2 - Navigating to _forked_ Repository
* Navigate to your github profile to find the _newly forked repository_.
* Copy the URL of the project to the clipboard.

#### Part 3 - Cloning _forked_ repository
* Clone the repository from **your account** into the `~/dev` directory.
  * if you do not have a `~/dev` directory, make one by executing the following command:
    * `mkdir ~/dev`
  * navigate to the `~/dev` directory by executing the following command:
    * `cd ~/dev`
  * clone the project by executing the following command:
    * `git clone https://github.com/MYUSERNAME/NAMEOFPROJECT`

#### Part 4 - Check Build
* Ensure that the tests run upon opening the project.
    * You should see `Tests Failed: 99 of 99 tests`







## How to Submit

#### Part 1 -  _Pushing_ local changes to remote repository
* from a _terminal_ navigate to the root directory of the _cloned_ project.
* from the root directory of the project, execute the following commands:
    * add all changes
      * `git add .`
    * commit changes to be pushed
      * `git commit -m 'I have added changes'`
    * push changes to your repository
      * `git push -u origin master`

#### Part 2 - Submitting assignment
* from the browser, navigate to the _forked_ project from **your** github account.
* click the `Pull Requests` tab.
* select `New Pull Request`
