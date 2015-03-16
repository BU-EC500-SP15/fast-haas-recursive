Usage: /home/sahil/git/haas/.venv/bin/haas <command> <arguments...> 
Where <command> is one of:
# **** Following calls need to be changed to CAll BASE HAAS ****
  headnode_connect_network <headnode> <nic> <network>
      Connect <headnode> to <network> on given <nic>
  headnode_create <headnode> <project> <base_img>
      Create a <headnode> in a <project> with <base_img>
  headnode_create_hnic <headnode> <nic>
      Create a <nic> on the given <headnode>
  headnode_delete <headnode>
      Delete <headnode>
  headnode_delete_hnic <headnode> <nic>
      Delete a <nic> on a <headnode>
  headnode_detach_network <headnode> <nic>
      Detach <headnode> from the network on given <nic>
  headnode_start <headnode>
      Start <headnode>
  headnode_stop <headnode>
      Stop <headnode>

# **** END OF SECTION **** 


  help <commands...>
      Display usage of all following <commands>, or of all commands if none are given
  init_db
      Initialize the database
  list_free_nodes
      List all free nodes
  list_headnode_images
      Display registered headnode images
  list_project_networks <project>
      List all networks attached to a <project>
  list_project_nodes <project>
      List all nodes attached to a <project>

# **** Following calls need to be changed to CAll BASE HAAS ****

  network_create <network> <creator> <access> <net_id>
      Create a link-layer <network>.  See docs/networks.md for details
  network_create_simple <network> <project>
      Create <network> owned by project.  Specific case of network_create
  network_delete <network>
      Delete a <network>

# **** END OF SECTION **** 


# **** Following calls need to be changed to CAll BASE HAAS ****
  node_connect_network <node> <nic> <network>
      Connect <node> to <network> on given <nic>

##  node_delete <node> 				# ** No need to change anything 
      Delete <node>
##   node_delete_nic <node> <nic> 	# ** No need to change anything 
      Delete a <nic> on a <node>
  node_detach_network <node> <nic>
      Detach <node> from the network on given <nic>
  node_power_cycle <node>
      Power cycle <node>
##  node_register <node> <ipmi_host> <ipmi_user> <ipmi_pass>						# ** No need to change anything 
      Register a node named <node>, with the given ipmi host/user/password 		
##  node_register_nic <node> <nic> <macaddr>										# ** No need to change anything 
      Register existence of a <nic> with the given <macaddr> on the given <node> 	

# **** END OF SECTION ****

 
#dont touch it 
 port_connect_nic <port> <node> <nic>
      Connect a <port> on a switch to a <nic> on a <node>
  port_delete <port>
      Delete a <port> on a switch
  port_detach_nic <port>
      Detach a <port> on a switch from whatever's connected to it
  port_register <port>
      Register a <port> on a switch


  project_add_user <project> <user>
      Add <user> to <project>
  project_connect_node <project> <node>
      Connect <node> to <project>
  project_create <project>
      Create a <project>
  project_delete <project>
      Delete <project>
  project_detach_node <project> <node>
      Detach <node> from <project>
  project_remove_user <project> <user>
      Remove <user> from <project>

  serve
      Start the HaaS API server
  serve_networks
      Start the HaaS networking server

# **** Following calls need to be changed to CAll BASE HAAS ****
  show_console <node>
      Display console log for <node>
  show_headnode <headnode>
      Display information about a <headnode>
##  show_node <node>							# ** No need to change anything 
      Display information about a <node>
  start_console <node>
      Start logging console output from <node>
  stop_console <node>
      Stop logging console output from <node> and delete the log
##  user_create <username> <password> 			# ** No need to change anything 
      Create a user <username> with password <password>.
##  user_delete <username> 						# ** No need to change anything 
      Delete the user <username>





