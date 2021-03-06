# Projects: Basic Data Structures and Algorithms
<!-- *Estimated Time: 6-10 hours* -->

*Don't forget to use Git to save your projects!*

## Project 1: Searching Binary Trees

You learned about [binary search trees](http://en.wikipedia.org/wiki/Binary_search_tree) -- where you take a group of data items and turn them into a tree full of nodes where each left node is "lower" than each right node.  The tree starts with the "root node" and any node with no children is called a "leaf node".

You also learned about tree search algorithms like breadth-first-search and depth-first-search.  You learned that BFS is best used to find the optimum solution but can take a very long time (impractically long for broad and deep data sets) while DFS is often much faster but will give you the FIRST solution, not necessarily the best.  Here you'll get a chance to implement both.

### Your Task

You'll build a simple binary tree data structure from some arbitrary input and also the "crawler" function that will locate data inside of it.

1. Build a class `Node`.  It should have a `value` that it stores and also links to its parent and children (if they exist).  Build getters and setters for it (e.g. parent node, child node(s)).
2. Write a method `build_tree` which takes an array of data (e.g. [1, 7, 4, 23, 8, 9, 4, 3, 5, 7, 9, 67, 6345, 324]) and turns it into a binary tree full of `Node` objects appropriately placed.  Start by assuming the array you get is sorted.
3. Now refactor your `build_tree` to handle data that isn't presorted and cannot be easily sorted prior to building the tree.  You'll need to figure out how to add a node for each of the possible cases (e.g. if it's a leaf versus in the middle somewhere).
3. Write a simple script that runs `build_tree` so you can test it out.
5. Build a method `breadth_first_search` which takes a target value and returns the node at which it is located using the breadth first search technique.  **Tip:** You will want to use an array acting as a queue to keep track of all the child nodes that you have yet to search and to add new ones to the list (as you saw in the [video](https://youtu.be/9RHO6jU--GU)).  If the target node value is not located, return `nil`.
4. Build a method `depth_first_search` which returns the node at which the target value is located using the depth first search technique.  Use an array acting as a *stack* to do this.
5. Next, build a new method `dfs_rec` which runs a depth first search as before but this time, instead of using a stack, make this method recursive.
6. Tips:

    1. You can think of the `dfs_rec` method as a little robot that crawls down the tree, checking if a node is the correct node and spawning other little robots to keep searching the tree.  No robot is allowed to turn on, though, until all the robots to its left have finished their task.
    2. The method will need to take in both the target value and the current node to compare against.

### Student Solutions

*Send us your solution so we can show others! Submit a link to the Github repo with your files in it here using any of the methods listed on the [contributing page](http://github.com/TheOdinProject/curriculum/blob/master/contributing.md).  Please include your partner's github handle somewhere in the description if they would like attribution.*

* Add your solution below this line!
* [Stefan P's solution](https://github.com/spavikevik/bst)
* [Donald's solution](https://github.com/donaldali/odin-ruby/tree/master/project_data_structs_alg/bst)
* [Mazin's solution](https://github.com/muzfuz/CodeLessons/blob/master/binary_search/binary_search.rb)
* [Marina Sergeyeva's solution](https://github.com/imousterian/OdinProject/blob/master/Project2_7_Ruby_DataStructures/binarytree.rb)
* [Tommy Noe's solution](https://github.com/thomasjnoe/bst-practice)
* [Michael Alexander's solution](https://github.com/betweenparentheses/project_data_structures/blob/master/binarytree.rb)
* [Sahil Agarwal's solution](https://github.com/sahilda/the_odin_project/tree/master/data-structures-and-algorithms)
* [Aleksandar's solution](https://github.com/Rodic/Odin-Ruby-Projects/blob/master/Projects:%20Basic%20Data%20Structures%20and%20Algorithms/lib/btree.rb)
* [John Quarles' solution](https://github.com/johnwquarles/Ruby-binary-trees-knights-travails/blob/master/binary_tree.rb)
* [Kate McFaul's solution](https://github.com/craftykate/odin-project/blob/master/Chapter_03-Advanced_Ruby/data_structures_and_algorithms/binary_search_tree.rb)
* [Artur Janik's solution](https://github.com/ArturJanik/TOPRuby/blob/master/Project7/BinTree/p1-tree.rb)
* [Jason Matthews' solution](https://github.com/fo0man/project_data_structures/blob/master/BinaryTree.rb)
* [Dominik Stodolny's solution](https://github.com/dstodolny/binary_tree/blob/master/binary_tree.rb)
* [Lara Finnegan's solution](https://github.com/lcf0285/algorithms/blob/master/binary_tree.rb)
* [Frank Peelen's solution](https://github.com/FrankPeelen/Data-Structures-and-Algorithms/blob/master/binary_search_tree.rb)
* [Brann James' solution](https://github.com/brannj/The_Odin_Project/blob/master/basic_data_structs/binary_trees.rb)
* [ll14m4n's solution](https://github.com/ll14m4n/the-odin-project/tree/master/3_Ruby_btree-search)
* [AtActionPark's solution](https://github.com/AtActionPark/odin_basic_data_structure/tree/master/lib)
* [Matias Pan's solution](https://github.com/kriox26/odin_ruby/tree/master/project_data_structures/bst)
* [Alex Chen's solution](https://github.com/Chenzilla/data_structure_practice)
* [Mark Viola's solution](https://github.com/markviola/the-odin-project/tree/master/12-data-structures-and-algorithms/1%20-%20Searching%20Binary%20Trees)
* [Xavier Reid's solution](https://github.com/xreid/data_structures_algorithms/tree/master/binary_tree)
* [Dan Hoying's solution](https://github.com/danhoying/basic_data_structures_and_algorithms/blob/master/searching_binary_trees.rb)
* [PiotrAleksander's solution](https://github.com/PiotrAleksander/Ruby/blob/master/drzewo_binarne.rb)
* [Florian Mainguy's solution](https://github.com/florianmainguy/theodinproject/blob/master/ruby/basic-data-structures-and-algorithms/searching_binary_tree.rb)
* [Sander Schepens's solution](https://github.com/schepens83/theodinproject.com/blob/master/ruby/project12--searching-binary-trees/searching_binary_trees.rb)
* [Noah Prescott's solution](https://github.com/npresco/basic_data_structures_and_algorithms/blob/master/binary_search.rb)
* [poctek's solution](https://github.com/poctek/The_Odin_Project/blob/master/Learning/CS/Algorithms/binary_tree.rb)
* [Aviv Levinsky's solution](https://github.com/pugsiman/Ruby_challenges_and_algorithms/blob/master/Searching_Binary_Trees/sbt.rb)
* [Giorgos's solution](https://github.com/vinPopulaire/search_binary_trees)
* [Andrew Park's solution](https://github.com/akpark93/the_odin_project/tree/master/ruby_programming_projects/Data%20Structures)
* [Scott Bobbitt's solution](https://github.com/sco-bo/binary_search_tree)
* [srashidi's solution](https://github.com/srashidi/Data_Structures/blob/master/Node/node.rb)
* [cdouglass's solution](https://github.com/cdouglass/odin-project-exercises/tree/master/ruby/data-structures-and-algorithms/binary_search_trees)
* [James Brooks's solution](https://github.com/jhbrooks/binary-search-tree)
* [Panashe Fundira's solution](https://github.com/munyari/odin/blob/master/learn-ruby/bfs_dfs/Node.rb)
* [Matt Velez's solution](https://github.com/Timecrash/ruby-projects/blob/master/data-structures/binary_tree.rb)
* [Luke Walker's solution](https://github.com/ubershibs/ruby-programming/blob/master/algorithms/binary_search.rb)
* [Miguel Herrera's solution](https://github.com/migueloherrera/projects/blob/master/binary_trees.rb)
* [Max Gallant's solution](https://github.com/mcgalcode/Ruby/tree/master/DataStructures)
* [Ricardo Villegas' solution](https://github.com/claricardo/RubyBuildingBlocks/blob/master/algorithms/binary_search_tree.rb)
* [Jack Wilde's solution](https://github.com/WildeRunner/data_structures_projects)
* [djhart's solution](https://github.com/djhart/binary_search)
* [Fabricio Carrara's solution](https://github.com/fcarrara/ruby_data_structures/blob/master/binary_search_tree.rb)
* [DV's solution](https://github.com/dvislearning/binary_search_tree/blob/master/bst.rb)
* [Earth35's solution](https://github.com/Earth35/binary_tree_search)
* [Stefan (Cyprium)'s solution](https://github.com/dev-cyprium/DataStructures-In-Ruby)
* [Shala Qweghen's solution](https://github.com/ShalaQweghen/basic_data_structure/blob/master/binary_trees.rb)
* [John Connor's solution](https://github.com/jacgitcz/binary_tree)
* [Jean Merlet's solution](https://github.com/jeanmerlet/data_structures/blob/master/binary_tree.rb)
* [Austin Mason's solution](https://github.com/CouchofTomato/algorithm/blob/master/binary_search_tree.rb)
* [Loris Aranda's solution](https://github.com/LorisProg/ruby-binary_search_tree-knight_travails/blob/master/binary_search_tree.rb)
* [Joanna Takesian's solution](https://github.com/joannatakesian/data-structures/blob/master/binary-tree/binary-tree.rb)
* [Francisco Carlos's solution](https://github.com/fcarlosdev/the_odin_project/tree/master/data_structures/binary_search_tree)
* [at0micred's solution](https://github.com/at0micr3d/data_structure)
* [Clint's solution](https://github.com/tholymap/OdinDataStructures/blob/master/bin_tree.rb)
* [Dylan's solution](https://github.com/resputin/the_odin_project/blob/master/Ruby/data_structures/bintree2.rb)
* [Leonard Soai-Van's solution](https://github.com/leosoaivan/TOP_compsci/blob/master/binary_tree.rb)
* [Dom Goj's solution](https://github.com/booyakuhhsha/linkedLists/commit/a3928f9747d422a49801e27e6d88b0cfc3fb3324)
* [Jerry Gao's solution](https://github.com/blackwright/odin/tree/master/ruby_binary_tree)
* [Sophia Wu's solution](https://github.com/SophiaLWu/project-basic-data-structs-and-algorithms/blob/master/binary_tree.rb)
* [Anthony Vumbaca's solution](https://github.com/tvumbaca/basic_data_structures/blob/master/binary_tree.rb)
* [Braydon Pacheco's solution](https://github.com/pacheeko/data_structures/blob/master/bst.rb)

## Project 2: Knight's Travails

Now you're a pro with DFS and BFS.  Let's try using our search algorithms on a real problem.

For this project, you'll need to use a data structure that's similar (but not identical) to a binary tree. For a summary of a few different examples, reference [this article](https://www.khanacademy.org/computing/computer-science/algorithms/graph-representation/a/describing-graphs).

A knight in chess can move to any square on the standard 8x8 chess board from any other square on the board, given enough turns (don't believe it?  See [this animation](http://upload.wikimedia.org/wikipedia/commons/c/ca/Knights-Tour-Animation.gif)).  Its basic move is two steps forward and one step to the side.  It can face any direction.

All the possible places you can end up after one move look like this:

<img src="http://0.tqn.com/d/chess/1/0/6/-/-/-/KnightMoves.gif">

### Your Task

Your task is to build a function `knight_moves` that shows the simplest possible way to get from one square to another by outputting all squares the knight will stop on along the way.

You can think of the board as having 2-dimensional coordinates.  Your function would therefore look like:

  * `knight_moves([0,0],[1,2]) == [[0,0],[1,2]]`
  * `knight_moves([0,0],[3,3]) == [[0,0],[1,2],[3,3]]`
  * `knight_moves([3,3],[0,0]) == [[3,3],[1,2],[0,0]]`

1. Put together a script that creates a game board and a knight.
2. Treat all possible moves the knight could make as children in a tree.  Don't allow any moves to go off the board.
2. Decide which search algorithm is best to use for this case.  Hint: one of them could be a potentially infinite series.
3. Use the chosen search algorithm to find the shortest path between the starting square (or node) and the ending square.  Output what that full path looks like, e.g.:

    ```language-bash
        > knight_moves([3,3],[4,3])
        You made it in 3 moves!  Here's your path:
        [3,3]
        [4,5]
        [2,4]
        [4,3]
    ```

### Student Solutions

*Send us your solution so we can show others! Submit a link to the Github repo with your files in it here using any of the methods listed on the [contributing page](http://github.com/TheOdinProject/curriculum/blob/master/contributing.md).  Please include your partner's github handle somewhere in the description if they would like attribution.*

* Add your solution below this line!
* [Stefan P's solution](https://github.com/spavikevik/knight_travails)
* [Leonard Soai-van's solution] (https://github.com/leosoaivan/TOP_compsci)
* [Donald's solution](https://github.com/donaldali/odin-ruby/tree/master/project_data_structs_alg/knights_travails)
* [Marina Sergeyeva's solution](https://github.com/imousterian/OdinProject/blob/master/Project2_7_Ruby_DataStructures/knight.rb)
* [Tommy Noe's solution](https://github.com/thomasjnoe/knight-moves)
* [Michael Alexander's solution](https://github.com/betweenparentheses/project_data_structures/blob/master/knightstravails.rb)
* [Sahil Agarwal's solution](https://github.com/sahilda/the_odin_project/tree/master/data-structures-and-algorithms)
* [Sergio Ribeiro's solution](https://github.com/serg1o/Data_Structures/blob/master/knight.rb)
* [Aleksandar's solution](https://github.com/Rodic/Odin-Ruby-Projects/blob/master/Projects:%20Basic%20Data%20Structures%20and%20Algorithms/lib/knight.rb)
* [John Quarles' solution](https://github.com/johnwquarles/Ruby-binary-trees-knights-travails/blob/master/knight.rb)
* [Kate McFaul's solution](https://github.com/craftykate/odin-project/blob/master/Chapter_03-Advanced_Ruby/data_structures_and_algorithms/knight_moves.rb)
* [Artur Janik's solution](https://github.com/ArturJanik/TOPRuby/blob/master/Project7/KnightsTravails/p2-knight.rb)
* [Jason Matthews' solution](https://github.com/fo0man/project_data_structures/blob/master/knight_travails.rb)
* [Dominik Stodolny's solution](https://github.com/dstodolny/knight_moves/blob/master/knight_moves.rb)
* [Lara Finnegan's solution](https://github.com/lcf0285/algorithms/blob/master/knights_travails.rb)
* [Frank Peelen's solution](https://github.com/FrankPeelen/Data-Structures-and-Algorithms/blob/master/knight_moves.rb)
* [Brann James' solution](https://github.com/brannj/The_Odin_Project/blob/master/basic_data_structs/knight_travails.rb)
* [ll14m4n's solution](https://github.com/ll14m4n/the-odin-project/tree/master/3_Ruby_khight-moves)
* [AtActionPark's solution](https://github.com/AtActionPark/odin_basic_data_structure/blob/master/knight_moves.rb)
* [Matias Pan's solution](https://github.com/kriox26/odin_ruby/tree/master/project_data_structures/knight_moves)
* [Alex Chen's solution](https://github.com/Chenzilla/data_structure_practice)
* [Mark Viola's solution](https://github.com/markviola/the-odin-project/tree/master/12-data-structures-and-algorithms/2%20-%20Knights%20Travail)
* [Xavier Reid's solution](https://github.com/xreid/data_structures_algorithms/blob/master/knights_travails/knight.rb)
* [Dan Hoying's solution](https://github.com/danhoying/basic_data_structures_and_algorithms/blob/master/knights_travails.rb)
* [PiotrAleksander's solution](https://github.com/PiotrAleksander/Ruby/blob/master/goniec.rb)
* [Florian Mainguy's solution](https://github.com/florianmainguy/theodinproject/blob/master/ruby/basic-data-structures-and-algorithms/knight.rb)
* [Sander Schepens's solution](https://github.com/schepens83/theodinproject.com/blob/master/ruby/project13--knights-travails/knights_travails.rb)
* [Noah Prescott's solution](https://github.com/npresco/basic_data_structures_and_algorithms/blob/master/knight_moves.rb)
* [Alex Tsiras' solution](https://github.com/arialblack14/binary_trees/blob/master/knight.rb)
* [Giorgos's solution](https://github.com/vinPopulaire/knights_travails)
* [Scott Bobbitt's solution](https://github.com/sco-bo/knights_travails)(w/help from John Quarles' blog post)
* [srashidi's solution](https://github.com/srashidi/Data_Structures/blob/master/Knights_Travails/knight_moves.rb)
* [cdouglass's solution](https://github.com/cdouglass/odin-project-exercises/tree/master/ruby/data-structures-and-algorithms/knights_travails)
* [James Brooks's solution](https://github.com/jhbrooks/knight-moves)
* [Panashe Fundira's solution](https://github.com/munyari/odin/blob/master/learn-ruby/bfs_dfs/knight_shortest_path.rb)
* [Matt Velez's solution](https://github.com/Timecrash/ruby-projects/blob/master/data-structures/knight_traversal.rb)
* [Luke Walker's solution](https://github.com/ubershibs/ruby-programming/blob/master/algorithms/knight_moves.rb)
* [Miguel Herrera's solution](https://github.com/migueloherrera/projects/blob/master/knights_travails.rb)
* [Tomasz Kula's solution](https://github.com/zetsnotdead/Knights-Travails) including visual representation of the steps
* [Max Gallant's solution](https://github.com/mcgalcode/Ruby/tree/master/DataStructures)
* [Ricardo Villegas' solution](https://github.com/claricardo/RubyBuildingBlocks/blob/master/algorithms/knight_moves.rb)
* [Jack Wilde's solution](https://github.com/WildeRunner/data_structures_projects)
* [djhart's solution](https://github.com/djhart/knight_path)
* [Fabricio Carrara's solution](https://github.com/fcarrara/ruby_data_structures/tree/master/knight_moves)
* [Earth35's solution](https://github.com/Earth35/knight_moves)
* [DV's solution](https://github.com/dvislearning/knight_travels/blob/master/knight_travels.rb)
* [Shala Qweghen's solution](https://github.com/ShalaQweghen/basic_data_structure/blob/master/knight_moves.rb)
* [John Connor's solution](https://github.com/jacgitcz/knight_moves)\
* [Jean Merlet's solution](https://github.com/jeanmerlet/ruby_games/blob/master/chess/knight_movement.rb)
* [Jiazhi Guo's solution](https://github.com/jerrykuo7727/knights_travails)
* [Austin Mason's solution](https://github.com/CouchofTomato/algorithm/blob/master/knights_travails.rb)
* [Loris Aranda's solution](https://github.com/LorisProg/ruby-binary_search_tree-knight_travails/blob/master/knight_moves.rb)
* [Francisco Carlos's solution](https://github.com/fcarlosdev/the_odin_project/tree/master/data_structures/knight_travails)
* [m-chrzan's solution](https://github.com/m-chrzan/knights-travails)
* [at0micred's solution](https://github.com/at0micr3d/data_structure)
* [Clint's solution](https://github.com/tholymap/OdinDataStructures/blob/master/knight_moves.rb)
* [Dylan's solution](https://github.com/resputin/the_odin_project/blob/master/Ruby/data_structures/knight.rb)
* [David Chapman's solution](https://github.com/davidchappy/odin_training_projects/tree/master/knights_travails)
* [Dom Goj's solution](https://github.com/booyakuhhsha/linkedLists/blob/master/knight2.rb)
* [Jerry Gao's solution](https://github.com/blackwright/odin/tree/master/ruby_knights_travails)
* [Sophia Wu's solution](https://github.com/SophiaLWu/project-basic-data-structs-and-algorithms/blob/master/knights_travails.rb)
* [Anthony Vumbaca's solution](https://github.com/tvumbaca/basic_data_structures/blob/master/knights_travails.rb)
* [Braydon Pacheco's solution](https://github.com/pacheeko/data_structures/blob/master/knights_travails.rb)
## Additional Resources

*This section contains helpful links to other content. It isn't required, so consider it supplemental for if you need to dive deeper into something*

* More on [Binary Search Trees from Coursera](https://www.youtube.com/watch?v=pJ6aeg8x1Ig)... it gets a bit technical.
