# MultipleActivityDemo
Passing variable and their values from one activity to another

<b>Sending from One Activty(MainActivity)</b>

 final Intent intent=new Intent(getApplicationContext(),SecondActivity.class); 
 <br/>//SecondActivity (Class which to which we are sending the data)
 <br/>
 <code>
  intent.putExtra("friendName",friends.get(position));
	
  startActivity(intent);
 </code>
 
 <b>Receiving in another activity(SecondActivity)</b>
 
 <code>
 Intent intent =getIntent();
 Toast.makeText(getApplicationContext(),intent.getStringExtra("friendName"),Toast.LENGTH_SHORT).show();
 </code>
