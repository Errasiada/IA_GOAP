# IA_GOAP

In this practice the main task is creating an Unity 3D project applying a GOAP system. A Goal Oriented Action Planning (GOAP) is an IA system that will easily give your agents choices and the tools to make smart decisions without having to maintain a large and complex finite state machine.

For this demo, there will be three Agent types. These are the actions that those Agents will take place:

- Customer Agent: 1. Arrive to the bar 2. Order Menu 3. Go to the table 4. Leave the bar

- Barman Agent: 1. Arrive to the kitchen 2. Prepare Menu 3. Serve Menu 4. Kick jehovas witnesses

- Jehovas Witness Agent: 1. Arrive to the bar 2. Disturb customers 3. Leave bar

- Delivery Man Agent: 1. Arrive to the bar 2. Deliver products 3. Leave bar

![Agent customer](https://user-images.githubusercontent.com/114673717/214602631-95edb4d4-fa4c-468a-8a43-ff544fc53ee3.png)


After deiciding the different agents and its behaviours, I created the map- There is the kitchen and bar area where the barman agent moves, the chairs and tables for the customer, and an exit and entrance area. Also, different prefabs as the characters. The yellow characters are the Customers, the black character is the Jehova Witness, and the orange character are the Barman - Delivery man.

![image](https://user-images.githubusercontent.com/114673717/214023532-ae85bd0d-9b48-4f3f-922f-5739b84f16cc.png)
Sample 1. Early scene.

After that, I created a NavMesh system and added a NavMesh Agent component to each one of the agents. The most important thing was planning everything the agents where supposed to do, and how would they deal with each other. Based on that, the mechanic is:

Barman arrives first to the bar and opens the kitchen, customers start arriving and ordering menu's while the barman prepares and serves them. Meanwhile, the Jehova Witness agent enters the scene and starts disturbing the customers, so the Barman goes and kicks him. During those actions there's a Delivery Man Spawner with a random number that enters the scene just to deliver packages and leave.

Here is a gif as sample of the project:

![demogoap](https://user-images.githubusercontent.com/114673717/214605643-2dff0ac1-4f80-497b-a6b7-c1e07bce81d0.gif)

