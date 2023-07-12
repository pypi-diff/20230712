# Comparing `tmp/b2sim-1.0.8.tar.gz` & `tmp/b2sim-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.8.tar", last modified: Mon Jul 10 20:01:11 2023, max compression
+gzip compressed data, was "b2sim-1.0.9.tar", last modified: Mon Jul 10 23:51:55 2023, max compression
```

## Comparing `b2sim-1.0.8.tar` & `b2sim-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.359218 b2sim-1.0.8/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.8/LICENSE
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.8/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-10 20:01:11.358216 b2sim-1.0.8/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    13115 2023-07-04 23:24:21.000000 b2sim-1.0.8/README.md
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.297161 b2sim-1.0.8/b2sim/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.8/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10431 2023-07-04 00:29:36.000000 b2sim-1.0.8/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.8/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)   102973 2023-07-05 03:18:50.000000 b2sim-1.0.8/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.8/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.356216 b2sim-1.0.8/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.8/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      413 2023-07-06 22:49:54.000000 b2sim-1.0.8/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.310173 b2sim-1.0.8/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-10 20:01:11.359218 b2sim-1.0.8/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-05 03:07:31.000000 b2sim-1.0.8/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:21.287904 b2sim-1.0.9/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.9/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.0.9/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-11 23:59:21.273824 b2sim-1.0.9/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    14173 2023-07-10 20:01:59.000000 b2sim-1.0.9/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:20.368952 b2sim-1.0.9/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.0.9/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10590 2023-07-11 16:22:42.000000 b2sim-1.0.9/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.9/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   105812 2023-07-11 23:53:37.000000 b2sim-1.0.9/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.9/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:21.158188 b2sim-1.0.9/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.9/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-11 02:24:19.000000 b2sim-1.0.9/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:20.853323 b2sim-1.0.9/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-11 23:59:21.292768 b2sim-1.0.9/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-10 22:20:35.000000 b2sim-1.0.9/setup.py
```

### Comparing `b2sim-1.0.8/LICENSE` & `b2sim-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.8/README.md` & `b2sim-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# Welcome!
+# Overview
 
-Hi there! I'm redlaserbm, the main developer of the BTDB2 Eco simulator. To get started with using the code, please read through this README file! 
+The `b2sim` Python library is an extensive feature-rich library for simulating flowcharts within battles 2. Simulating essential aspects of battles 2's income sources with virtually 100% accuracy, the library is a must-use tool for optimizing eco'ing and farming with any flowchart. Results from the simulator can be used to better inform practical decisions made during games, improving player game sense and leading to more optimal play. The code is relatively easy to use and does not require prior coding experience to effectively operate.
 
-- To learn how to operate the code, see the examples folder.
+- To install the code, first download Python on your machine, and then in the terminal type `pip install b2sim` and hit 'Enter'.
+- To learn how to operate the code, see the examples folder in this GitHub repo. It contains numerous examples with code explained in plain English.
 - Want to request features for the code? Want to help out with the code? Found a bug? Don't hesitate to contact me! The most immediate way to get my attention with regards to this code is to join the b2 Popology discord server and ping me there: https://discord.gg/axHnkcVe6E
 - Potential collaborators interested with helping out with the code should view the "Feature Requests" section below for more info on tasks that need to be completed.
 
 # Operating the Code
 
 To run the code, do the following: 
 1. Install python on your computer. 
@@ -18,14 +19,17 @@
 
 1. **Simultaneous simulation of eco, farms, and alt-eco:** When given an eco send to use and some arrangement of farms and alt-eco, the simulator accurately tracks the progression of the player's cash and eco over time. The results of the simulator are nearly true to the game.
 2. **Easy operation:** Simply input your initial cash and eco, the round to start on, and the purchases you intend to make and the eco flowchart you intend to follow over the course of the match. The code runs in one click and delivers results in seconds.
 3. **Complete Farm support:** The simulator supports IMF Loans and Monkeyopolis. Also, the simulator supports compound purchases, such as selling into Monkey Wall Street.
 4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game. 
 
 # Update Log
+- (July 4, 2023 - v1.0.7)
+   - Fixed various bugs which caused the simulator to behave incorrectly when fail-safes were triggered. Such issues were related to when the eco sim tried to change eco sends as a consequence of a break condition (such as `max_eco_amount`) on the current send being satisfied.
+   - Updated display for graphs. The legend shows (approximated to the nearest tenth) when each action is carried out in the simulation.
 - (July 2, 2023 - v1.0.6)
    - Fixed an issue which effectively caused the attack queue size to be 5 instead of 6.
    - New action `sellAllFarms` for rapidly selling all farms.
 - (July 2, 2023 - v1.0.5)
    - Improved support for eco numbers. It is no longer mandatory when specifying eco sends in the eco queue to specify a time for the player to start triggering that send. Note that if you place a send in the queue without a time specified, the previous send must have some sort of break condition (like `max_eco_amount` or `max_send_amount`) specified which compels the simulator to switch sends, otherwise the next send in the queue will never be triggered.
 - (July 1, 2023 - v1.0.4)
    - Fixed an issue which caused the attack queue (which concerns the queue of bloons sent to your opponent) to sometimes fail to remove sends from the queue that already finished sending, resulting in the simulator computing incorrect eco amounts during simulation.
```

### Comparing `b2sim-1.0.8/b2sim/actions.py` & `b2sim-1.0.9/b2sim/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,21 @@
         'Minimum Buy Time': min_buy_time #Okay, this might be confusing, but this is actually the minimum *sell* time for this action.
     }
 
 # WARNING: This function is for declaring boat farms in the initial game state. 
 # Do NOT use it to add boat farms during simulation
 def initBoatFarm(purchase_time = None, upgrade = 3):
     return {
+        'Initial Purchase Time': purchase_time,
         'Purchase Time': purchase_time,
         'Upgrade': upgrade,
+        'Revenue': 0,
+        'Expenses': 0,
+        'Hypothetical Revenue': 0,
+        'Sell Time': None
     }
 
 #############
 # DRUID FARMS
 #############
 
 def buyDruidFarm(buffer = 0, min_buy_time = 0):
```

### Comparing `b2sim-1.0.8/b2sim/info.py` & `b2sim-1.0.9/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.8/b2sim/main.py` & `b2sim-1.0.9/b2sim/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,15 @@
 
         #I'll use this list to track the amount of money each farm makes over the course of the simulation
         self.farm_revenues = []
         self.farm_expenses = []
 
         #These lists will hold tuples (time, message)
         #These tuples are utilized by the viewCashAndEcoHistory method to display detailed into to the player about what actions were taken at what during simulation
-        self.buy_messages = []
-        self.eco_messages = []
+        self.event_messages = []
         
         #~~~~~~~~~~~~~~~
         #FARMS & ALT-ECO
         #~~~~~~~~~~~~~~~
         
         #Process the initial info given about farms/alt-eco:
         
@@ -96,30 +95,29 @@
         
         #First, farms!
 
         # We assume in the initial state dictionary that there is an entry "Farms" consisting of a list of dictionaries.
         # Note that the structure of self.farms however is not a list, but a dictionary with keys being nonnegative integers
         # The rationale for doing this is to drastically simplify code related to performing compound transactions.
 
-        self.farms = {}
+        self.farms = []
         farm_info = initial_state.get('Farms')
-        self.key = 0
         if farm_info is not None:
             for farm_info_entry in farm_info:
-                self.farms[self.key] = MonkeyFarm(farm_info_entry)
+                self.farms.append(MonkeyFarm(farm_info_entry))
                 
                 #If the farm is a T5 farm, modify our T5 flags appropriately
                 #Do not allow the user to initialize with multiple T5's
                 for i in range(3):
-                    if self.farms[self.key].upgrades[i] == 5 and self.T5_exists[i] == False:
+                    if self.farms[-1].upgrades[i] == 5 and self.T5_exists[i] == False:
                         self.T5_exists[i] = True
-                    elif self.farms[self.key].upgrades[i] == 5 and self.T5_exists[i] == True:
-                        self.farms[self.key].upgrades[i] = 4
-                
-                self.key += 1
+                    elif self.farms[-1].upgrades[i] == 5 and self.T5_exists[i] == True:
+                        self.logs.append("Warning! The initial state contained multiple T5 farms. Modifying the initial state to prevent this.")
+                        self.warnings.append(len(self.logs)-1)
+                        self.farms[-1].upgrades[i] = 4
 
         #Next, boat farms!
         boat_info = initial_state.get('Boat Farms')
         self.Tempire_exists = False
         self.boat_farms = {}
         self.boat_key = 0
         if boat_info is not None:
@@ -190,14 +188,16 @@
 
         self.eco_queue = initial_state.get('Eco Queue')
         if self.eco_queue is None:
             self.eco_queue = []
         self.number_of_sends = 0
 
         eco_send = initial_state.get('Eco Send')
+        if eco_send is None:
+            eco_send = ecoSend(send_name = 'Zero')
         eco_send['Time'] = 0
         self.eco_queue.insert(0,eco_send)
         
         #Upgrade queue
         self.buy_queue = initial_state.get('Buy Queue')
         self.buy_cost = None
         self.buffer = 0
@@ -246,105 +246,128 @@
         self.logs.append("The current game time is %s seconds"%(self.current_time))
         self.logs.append("The game round start times are given by %s \n"%(self.rounds.round_starts))
         
     def viewCashEcoHistory(self, dim = (15,18), display_farms = True, font_size = 12):
         self.logs.append("MESSAGE FROM GameState.viewCashEcoHistory():")
         self.logs.append("Graphing history of cash and eco!")
 
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        #Create a table that shows when each significant event in simulation occurs
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+        event_df = pd.DataFrame(self.event_messages)
+        event_df = event_df.round(1)
+        display(event_df)
+
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Graph the cash and eco values over time
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-        fig, ax = plt.subplots(1,2)
+        #Graphing cash
+        fig, ax1 = plt.subplots()
         fig.set_size_inches(dim[0],dim[1])
-        ax[0].plot(self.time_states, self.cash_states, label = "Cash")
-        ax[1].plot(self.time_states, self.eco_states, label = "Eco")
-        
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        #Mark where the rounds start
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+        color = 'tab:blue'
+        ax1.set_xlabel('Time (seconds)')
+        ax1.set_ylabel('Cash', color = color)
+        ax1.plot(self.time_states, self.cash_states, label = "Cash", color = color)
+        ax1.tick_params(axis ='y', labelcolor = color)
+
+        #Graphing eco
+        color = 'tab:orange'
+        ax2 = ax1.twinx()
+        ax2.set_ylabel('Eco', color = color)
+        ax2.plot(self.time_states, self.eco_states, label = "Eco", color = color)
+        ax2.tick_params(axis ='y', labelcolor = color)
+
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        #Mark on the graph messages in self.event_messages
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         cash_min = min(self.cash_states)
         eco_min = min(self.eco_states)
         
         cash_max = max(self.cash_states)
         eco_max = max(self.eco_states)
 
-        round_to_graph = self.rounds.getRoundFromTime(self.time_states[0]) + 1
-        while self.rounds.round_starts[round_to_graph] <= self.time_states[-1]:
-            ax[0].plot([self.rounds.round_starts[round_to_graph], self.rounds.round_starts[round_to_graph]],[cash_min-1, cash_max+1], label = "R" + str(round_to_graph) + " start", linestyle='dotted', color = 'k')
-            ax[1].plot([self.rounds.round_starts[round_to_graph], self.rounds.round_starts[round_to_graph]],[eco_min-1, eco_max+1], label = "R" + str(round_to_graph) + " start", linestyle='dotted', color = 'k')
-            round_to_graph += 1
-
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        #Mark where purchases in the buy queue and eco queue occurred
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        for message in self.event_messages:
 
-        for message in self.buy_messages:
-            if message[2] == 'Eco':
+            # Set different line properties for each message type
+            if message['Type'] == 'Eco':
+                line_style = ':'
                 line_color = 'b'
-            elif message[2] == 'Buy':
+            elif message['Type'] == 'Buy':
+                line_style = ':'
                 line_color = 'r'
-
-            if len(message[1]) > 30:
-                thing_to_say = message[1][0:22] + '...'
+            elif message['Type'] == 'Round':
+                line_style = ':'
+                line_color = 'k'
+
+            # If the given message is too long, truncate it.
+            if len(message['Message']) > 30:
+                thing_to_say = message['Message'][0:22] + '...'
             else:
-                thing_to_say = message[1]
-            
-            thing_to_say = thing_to_say + ' (R' + str(np.round(self.rounds.getRoundFromTime(message[0], get_frac_part = True),1)) + ')'
-            ax[0].plot([message[0],message[0]],[cash_min-1, cash_max+1], label = thing_to_say, linestyle = 'dashed', color = line_color)
-            ax[1].plot([message[0],message[0]],[eco_min-1, eco_max+1], label = thing_to_say, linestyle = 'dashed', color = line_color)
+                thing_to_say = message['Message']
+
+            #On both the cash and eco history graphs
+            ax1.plot([message['Time'],message['Time']],[cash_min-1, cash_max+1], label = thing_to_say, linestyle = line_style, color = line_color)
 
         #~~~~~~~~~~~~~~~~
         #Label the graphs
         #~~~~~~~~~~~~~~~~
 
-        ax[0].set_title("Cash vs Time")
-        ax[1].set_title("Eco vs Time")
-        
-        ax[0].set_ylabel("Cash")
-        ax[1].set_ylabel("Eco")
-        
-        ax[0].set_xlabel("Time (seconds)")
-        ax[1].set_xlabel("Time (seconds)")
-
-        ax[1].legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
-        
+        ax1.set_title("Cash & Eco vs Time")
+        ax1.legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
         fig.tight_layout()
 
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        #Create a table that displays the revenue made by each farm
-        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        #Create a table that displays the revenue/expenses of each farm
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         #Create a list of revenues and expenses for every farm
         self.farm_revenues = []
         self.farm_expenses = []
         self.farm_profits = []
         self.farm_eis = []
+        self.farm_starts = []
+        self.farm_ends = []
 
-        for key in self.farms.keys():
-            farm = self.farms[key]
+        for farm in self.farms:
             self.farm_revenues.append(farm.revenue)
             self.farm_expenses.append(farm.expenses)
             self.farm_profits.append(farm.revenue - farm.expenses)
 
             #Also, measure the equivalent eco impact of the farm
+            start_time = max(farm.init_purchase_time, self.simulation_start_time)
             if farm.sell_time == None:
-                self.farm_eis.append(6*farm.revenue/(self.current_time - max(farm.init_purchase_time, self.simulation_start_time)))
+                end_time = self.current_time
             else:
-                self.farm_eis.append(6*farm.revenue/(farm.sell_time -  max(farm.init_purchase_time, self.simulation_start_time)))
-                
+                end_time = farm.sell_time
+
+            self.farm_starts.append(start_time)
+            self.farm_ends.append(end_time)
+
+            self.farm_eis.append(6*farm.revenue/(end_time - start_time))
 
         # dictionary of lists 
         if display_farms and len(self.farms) > 0:
-            farm_table = {'Farm Index': [int(i) for i in range(self.key)], 'Revenue': self.farm_revenues, 'Expenses': self.farm_expenses, 'Profit': self.farm_profits, 'Eco Impact': self.farm_eis} 
+            farm_table = {
+                'Farm Index': [int(i) for i in range(len(self.farms))], 
+                'Revenue': self.farm_revenues, 
+                'Expenses': self.farm_expenses, 
+                'Profit': self.farm_profits, 
+                'Eco Impact': self.farm_eis, 
+                'Start Time': self.farm_starts, 
+                'End Time': self.farm_ends
+            } 
             df = pd.DataFrame(farm_table)
             df = df.set_index('Farm Index')
             df = df.round(0)
             display(df)
+
         
         self.logs.append("Successfully generated graph! \n")
     
     def changeStallFactor(self,stall_factor):
         #NOTE: This method currently does not see use at all. It may be removed in a future update.
         self.rounds.changeStallFactor(stall_factor,self.current_time)
 
@@ -508,39 +531,57 @@
         self.max_send_amount = send_info['Max Send Amount']
         self.number_of_sends = 0
 
         #Setting the max_eco_amount
         self.max_eco_amount = send_info['Max Eco Amount']
 
         self.logs.append("Modified the eco send to %s"%(self.send_name))
-        self.buy_messages.append((self.current_time, 'Change eco to %s'%(self.send_name), 'Eco'))
+        self.event_messages.append({
+            'Time': self.current_time, 
+            'Type': "Eco",
+            'Message': "Change eco to %s"%(self.send_name)
+        })
 
     def showWarnings(self,warnings):
         for index in warnings:
             print(self.logs[index])
         
     def fastForward(self, target_time = None, target_round = None, interval = 0.1):
         self.logs.append("MESSAGE FROM GameState.fastForward: ")
         self.valid_action_flag = True #To prevent the code from repeatedly trying to perform a transaction that obviously can't happen
         self.simulation_start_time = self.current_time
         
         # If a target round is given, compute the target_time from that
         if target_round is not None:
             target_time = self.rounds.getTimeFromRound(target_round)
+
+        # Append messages to the event messages list showing when each round starts
+        given_round = self.current_round
+        end_round = self.rounds.getRoundFromTime(target_time)
+        while given_round <= end_round:
+            self.event_messages.append({
+                'Time': self.rounds.getTimeFromRound(given_round),
+                'Type': "Round",
+                'Message': "Round %s start"%(given_round)
+            })
+            given_round += 1
             
         #A fail-safe to prevent the code from trying to go backwards in time
         if target_time < self.current_time:
             target_time = self.current_time
         
         while self.current_time < target_time:
             intermediate_time = min(max(np.floor(self.current_time/interval + 1)*interval,self.current_time + interval/2),target_time)
             self.logs.append("Advancing game to time %s"%(np.round(intermediate_time,3)))
             self.advanceGameState(target_time = intermediate_time)
             self.logs.append("----------")
 
+        # Sort the messages in self.event_messages so that they are listed chronologically
+        self.event_messages = sorted(self.event_messages, key=lambda x: x['Time']) 
+
         #FOR SPOONOIL: Show warning messages for fail-safes triggered during simulation
         self.showWarnings(self.warnings)
         
         self.logs.append("Advanced game state to round " + str(self.current_round))
         self.logs.append("The current time is " + str(self.current_time))
         self.logs.append("The next round starts at time " + str(self.rounds.round_starts[self.current_round+1]))
         self.logs.append("Our new cash and eco is given by (%s,%s) \n"%(np.round(self.cash,2),np.round(self.eco,2)))
@@ -564,17 +605,16 @@
         if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] < target_time:
             #Yes, an eco change will occur
             target_time = self.eco_queue[0]['Time']
 
         # FAIL-SAFE: Check whether the current eco send is valid. If it is not, change the eco send to zero.
         if eco_send_info[self.send_name]['End Round'] < self.current_round:
             self.logs.append("Warning! The eco send %s is no longer available! Switching to the zero send."%(self.send_name))
-            self.logs.append("Warning! This message should not have come up during simulation! Please contact redlaserbm with information on what happened.")
             self.warnings.append(len(self.logs) - 1)
-            self.eco_queue.insert(0,{'Time': 0, 'Send Name': 'Zero'})
+            self.eco_queue.insert(0,ecoSend(time = 0, send_name='Zero'))
             target_time = self.eco_queue[0]['Time']
 
         # FAIL-SAFE: Prevent advanceGameState from using an eco send after it becomes unavailable by terminating early in this case.
         if eco_send_info[self.send_name]['End Round'] + 1 <= self.rounds.getRoundFromTime(target_time):
             target_time = self.rounds.getTimeFromRound(eco_send_info[self.send_name]['End Round'] + 1)
             self.logs.append("Warning! The current eco send will not be available after the conclusion of round %s. Adjusting the target time."%(eco_send_info[self.send_name]['End Round']))
 
@@ -881,16 +921,15 @@
                         'Source': 'Heli'
                     }
                     payout_times.append(payout_entry)
                     heli_farm_time += heli_globals['Heli Farm Usage Cooldown']
 
         #FARMS
         if len(self.farms) > 0:
-            for key in self.farms.keys():
-                farm = self.farms[key]
+            for key, farm in enumerate(self.farms):
                 if farm.sell_time is None:
                     #If the farm is a monkeynomics, determine the payout times of the active ability
                     if farm.upgrades[1] == 5:
                         farm_time = farm.min_use_time
                         while farm_time <= target_time:
                             if farm_time > self.current_time:
                                 payout_entry = {
@@ -992,26 +1031,35 @@
                                 self.flag = True
                                 break
                         self.inc += 1
         
         #BOAT FARMS
         if len(self.boat_farms) > 0:
 
-            #If the player has Trade Empire, determine the buff to be applied to other boat farm payments
+            #Is there a Trade Empire on screen right now? 
             if self.Tempire_exists == True:
-                arg = min(len(self.boat_farms) - 1,20)
+                #Yes, determine the buff to be applied to other boat farm payments.
+                active_boats = 0
+                for key in self.boat_farms.keys():
+                    boat_farm = self.boat_farms[key]
+                    if boat_farm['Sell Time'] is None:
+                        active_boats += 1
+                arg = min(active_boats - 1,20)
             else:
+                #No, there is not.
                 arg = 0
+
             multiplier = 1 + 0.05*arg
 
             #Determine the amount of the money the boats will give each round
             boat_payout = 0
             for key in self.boat_farms.keys():
                 boat_farm = self.boat_farms[key]
-                boat_payout += multiplier*boat_payout_values[boat_farm['Upgrade'] - 3]
+                if boat_farm['Sell Time'] is None:
+                    boat_payout += multiplier*boat_payout_values[boat_farm['Upgrade'] - 3]
 
             #At the start of each round, append a payout entry with the boat payout
             self.inc = 1
             while self.rounds.getTimeFromRound(self.current_round + self.inc) <= target_time:
                 payout_entry = {
                     'Time': self.rounds.getTimeFromRound(self.current_round + self.inc),
                     'Payout Type': 'Direct',
@@ -1042,14 +1090,15 @@
             'Payout': 0,
             'Source': 'Ghost',
         }
         payout_times.append(payout_entry)
 
         #Now that we determined all the payouts, sort the payout times by the order they occur in
         payout_times = sorted(payout_times, key=lambda x: x['Time']) 
+
         #self.logs.append("Sorted the payouts in order of increasing time!")
 
         return payout_times
 
     def updateEco(self, target_time):
         # Helper method which updates eco from the current game time to the specified target_time.
         # self.logs.append("Running updateEco!")
@@ -1162,17 +1211,22 @@
                 break
             
             # Next, let's compute the cash and loan values we would have if the transaction was performed
             # We will compute the hypothetical revenues each farm would have if the transactions were carried out
             # In general the this step is necessary if there are in the presence of loans.
             # NOTE: Loans do not influence purchases, so we can process expense tracking for farms only when a transaction actually occurs.
 
-            for key in self.farms.keys():
-                farm = self.farms[key]
+            #For tracking the revenue of farms
+            for farm in self.farms:
                 farm.h_revenue = farm.revenue
+
+            #For tracking the revenue of boat farms
+            for key in self.boat_farms.keys():
+                boat_farm = self.boat_farms[key]
+                boat_farm['Hypothetical Revenue'] = boat_farm['Revenue']
             
             for dict_obj in purchase_info:
 
                 # DEFENSE RELATED MATTERS
                 if dict_obj['Type'] == 'Buy Defense':
                     h_cash, h_loan = impact(h_cash, h_loan, -1*dict_obj['Cost'])
                     
@@ -1209,16 +1263,15 @@
                         h_cash, h_loan = h_new_cash, h_new_loan
                     else:
                         self.logs.append("WARNING! Tried to sell a farm that is not on screen! Aborting buy queue")
                         self.warnings.append(len(self.logs)-1)
                         self.valid_action_flag = False
                         break
                 elif dict_obj['Type'] == 'Sell All Farms':
-                    for key in self.farms.keys():
-                        farm = self.farms[key]
+                    for farm in self.farms:
                         if farm.sell_time is None:
                             h_new_cash, h_new_loan = impact(h_cash, h_loan, farm_sellback_values[tuple(farm.upgrades)])
                             farm.h_revenue += h_new_cash - h_cash
                             h_cash, h_loan = h_new_cash, h_new_loan
 
 
                 elif dict_obj['Type'] == 'Withdraw Bank':
@@ -1282,15 +1335,26 @@
                         self.valid_action_flag = False
                         break
                     upgrade_cost = boat_upgrades_costs[boat_farm['Upgrade']-3]
                     h_cash, h_loan = impact(h_cash, h_loan, -1*upgrade_cost)
                 elif dict_obj['Type'] == 'Sell Boat Farm':
                     ind = dict_obj['Index']
                     boat_farm = self.boat_farms[ind]
-                    h_cash, h_loan = impact(h_cash, h_loan, boat_sell_values[boat_farm['Upgrade']-3])
+
+                    #Check whether the boat farm is actually on screen before selling it:
+                    if boat_farm['Sell Time'] is None:
+                        #Selling a farm counts as that farm generating revenue
+                        h_new_cash, h_new_loan = impact(h_cash, h_loan, boat_sell_values[boat_farm['Upgrade']-3])
+                        boat_farm['Hypothetical Revenue'] += h_new_cash - h_cash
+                        h_cash, h_loan = h_new_cash, h_new_loan
+                    else:
+                        self.logs.append("WARNING! Tried to sell a boat farm that is not on screen! Aborting buy queue")
+                        self.warnings.append(len(self.logs)-1)
+                        self.valid_action_flag = False
+                        break
 
                 # DRUID FARM RELATED MATTERS
                 elif dict_obj['Type'] == 'Buy Druid Farm':
                     h_cash, h_loan = impact(h_cash, h_loan, -1*druid_globals['Druid Farm Cost'])
                 elif dict_obj['Type'] == 'Sell Druid Farm':
                     if dict_obj['Index'] == self.sotf:
                         h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(druid_globals['Druid Farm Cost'] + druid_globals['Spirit of the Forest Upgrade Cost']))
@@ -1366,18 +1430,22 @@
                 self.logs.append("We have %s cash! We can do the next buy, which costs %s and has a buffer of %s and a minimum buy time of %s!"%(np.round(self.cash,2), np.round(self.cash - h_cash,2),np.round(self.buffer,2),np.round(self.min_buy_time,2)))
 
                 # Make the adjustments to the cash and loan amounts
                 self.cash = h_cash
                 self.loan = h_loan
 
                 # Track the revenue made by each farm
-                for key in self.farms.keys():
-                    farm = self.farms[key]
+                for farm in self.farms:
                     farm.revenue = farm.h_revenue
 
+                # Track the revenue made by each boat farm
+                for key in self.boat_farms.keys():
+                    boat_farm = self.boat_farms[key]
+                    boat_farm['Revenue'] = boat_farm['Hypothetical Revenue']
+
                 # self.logs.append("The new lists of farm revenues and expenses are given by: ")
                 # self.logs.append(str(self.farm_revenues))
                 # self.logs.append(str(self.farm_expenses))
 
                 for dict_obj in purchase_info:
 
                     buy_message_list.append(dict_obj['Message'])
@@ -1386,17 +1454,15 @@
                     if dict_obj['Type'] == 'Buy Farm':
                         self.logs.append("Purchasing farm!")
                         farm_info = {
                             'Purchase Time': self.current_time,
                             'Upgrades': [0,0,0]
                         }
                         farm = MonkeyFarm(farm_info)
-                        
-                        self.farms[self.key] = farm
-                        self.key+= 1
+                        self.farms.append(farm)
 
                         #For revenue and expense tracking
                         farm.revenue = 0
                         farm.expenses = farm_globals['Farm Cost']
                         
                     elif dict_obj['Type'] == 'Upgrade Farm':
                         ind = dict_obj['Index']
@@ -1463,16 +1529,15 @@
 
                         #Mark the farm's sell time. The code checks whether this value is a number or not before trying to compute farm payments
                         farm.sell_time = payout['Time']
                         
                     elif dict_obj['Type'] == 'Sell All Farms':
                         self.logs.append("Selling all farms!")
                         self.T5_exists = [False for i in range(3)] #Obviously, if we sell all farms we won't have any T5's anymore!
-                        for key in self.farms.keys():
-                            farm = self.farms[key]
+                        for farm in self.farms:
                             farm.sell_time = payout['Time']
                     
                     elif dict_obj['Type'] == 'Withdraw Bank':
                         self.logs.append("Withdrawing money from the bank at index %s"%(ind))
                         ind = dict_obj['Index']
                         farm = self.farms[ind]
                         farm.account_value = 0
@@ -1482,25 +1547,33 @@
                         self.logs.append("Taking out a loan from the IMF at index %s"%(ind))
                         farm.min_use_time = payout['Time'] + farm_globals['IMF Usage Cooldown']
                         
                     # BOAT FARM RELATED MATTERS
                     elif dict_obj['Type'] == 'Buy Boat Farm':
                         self.logs.append("Purchasing boat farm!")
                         boat_farm = {
+                            'Initial Purchase Time': self.current_time,
                             'Purchase Time': self.current_time,
-                            'Upgrade': 3
+                            'Upgrade': 3,
+                            'Revenue': 0,
+                            'Expenses': boat_globals['Merchantmen Cost'],
+                            'Hypothetical Revenue': 0,
+                            'Sell Time': None
                         }
                         self.boat_farms[self.boat_key] = boat_farm
                         self.boat_key += 1
                     elif dict_obj['Type'] == 'Upgrade Boat Farm':
                         ind = dict_obj['Index']
                         
                         self.logs.append("Upgrading the boat farm at index %s"%(ind))
                         boat_farm = self.boat_farms[ind]
                         boat_farm['Upgrade'] += 1
+
+                        #Expense tracking
+                        boat_farm['Expenses'] += boat_upgrades_costs[boat_farm['Upgrade'] - 4]
                         
                         #Update the payout information of the boat farm
                         boat_farm['Payout'] = boat_payout_values[boat_farm['Upgrade'] - 3]
                         
                         #So that we can accurately track payments for the boat farm
                         boat['Purchase Time'] = payout['Time']
                         
@@ -1515,15 +1588,17 @@
                     elif dict_obj['Type'] == 'Sell Boat Farm':
                         ind = dict_obj['Index']
                         self.logs.append("Selling the boat farm at index %s"%(ind))
                         #If the farm being sold is a Trade Empire, indicate as such
                         if boat_farm['Upgrade'] == 5:
                             self.logs.append("The boat farm we're selling is a Trade Empire! Removing the Tempire buff.")
                             self.Tempire_exists = False
-                        self.boat_farms.pop(ind)
+
+                        #Mark the boat farm's sell time
+                        boat_farm['Sell Time'] = payout['Time']
 
                     # DRUID FARMS
                     elif dict_obj['Type'] == 'Buy Druid Farm':
                         self.druid_farms[self.druid_key] = payout['Time']
                         self.druid_key += 1
                         self.logs.append("Purchased a druid farm!")
                     elif dict_obj['Type'] == 'Sell Druid Farm':
@@ -1611,15 +1686,19 @@
                 #If we can't afford the buy, break the while loop
                 #self.logs.append("We can't afford the buy! Terminating the buy queue while loop")
                 break
         
         #...so that players can see where in the graphs their purchases are occuring
         if len(buy_message_list) > 0:
             buy_message = ', '.join(buy_message_list)
-            self.buy_messages.append((payout['Time'], buy_message, 'Buy'))
+            self.event_messages.append({
+                'Time': payout['Time'], 
+                'Type': "Buy", 
+                'Message': buy_message
+            })
         
         return made_purchase
             
 # %% [markdown]
 # Now it's time to define the MonkeyFarm class!
 
 # %%
```

### Comparing `b2sim-1.0.8/b2sim/rounds.py` & `b2sim-1.0.9/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.8/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.9/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

