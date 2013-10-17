## "it's time to kick ass and chew bubble gum...", </br>a unity 3D live coding demo


--
## Debug.log(this);

@David_Hodgetts  
demainlalune.ch

Note:
started using unity for media design projects
Unity is used in more than games (media design, serious gaming)
sae teacher
--


<br/>
## Unity 3d from a dev point of view

<p class="fragment">c++ engine</p>
<p class="fragment">scripting provided by Mono (open source .Net)</p>
<p class="fragment">c#, unityScript, boo</p>

--
## mono is actually an interesting choice

<p class="fragment">mono 2.6 (approx .Net 3.5)</p>
<p class="fragment">code completion, refactoring tools (works best with visual studio)</p>
<p class="fragment">access to .Net (sockets, XML, etc.)</p>
<p class="fragment">LINQ</p>

--
## How does it work?

--
## Once upon a time (old shool OO)

<p class="fragment">everything inherits from a base gameobject</p>
<p class="fragment">results in a tree of doom (vertical complexity)</p>
<p class="fragment">![](/images/evil_tree.png)</p>

--
## composition over inheritance
<p class="fragment">Component Entity Systems</p>
<p class="fragment">configurable, reusable, better encapsulated</p>
<p class="fragment">![](/images/flat_tree.png)</p>
--
## Entity
<p class="fragment">just an id</p>
<p class="fragment">with a container of components</p>
<p class="fragment">in Unity they are called GameObjects</p>
--
## Component
<p class="fragment">a minimal set of data needed for a specific purpose (SRP)</p>
<p class="fragment">an Object of Type MonoBehavior in Unity</p>
<p class="fragment">Transform, Material, Collider, and your own scripts</p>
--
## Systems
<p class="fragment">single purpose function that traverse the entities, and update each component</p>
<p class="fragment">the game loop and its events</p>
<p class="fragment">![](/images/unity_lifetime.png)</p>
--
## an interesting read

http://www.chris-granger.com/2012/12/11/anatomy-of-a-knockout/

--
## resources 
  
- embedded Asset Store
- http://www.reddit.com/r/Unity3D/ (links on the left)
--
## let's code




