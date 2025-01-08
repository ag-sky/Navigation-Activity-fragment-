# Navigation-Activity-fragment-

Navigation in between activities, this we can do via intents, 

Activity A, Activity B

val intent = Intent(this. ActivityB::class.java)
intent.putExtra("key,"value)
startActivity(intent)


Navivation in fragments, two methods ( fragments transactions, navigation component ( part of android jetpack) need to give dependencies.

val fragmentTransaction = requireActivity.supportfragmentmanager.begintransaction;
val fragmentB = FragmentB();
val bundle = Bundle();
bundle.putSstring(key,value)
bundle.arguments(bundle);
fragmenttransaction.replace(container.id, fragmentB)
fragmentranction.addtobackstack(null)
fragmenttranciton.commit();

val data = arguments?.getString(key)
