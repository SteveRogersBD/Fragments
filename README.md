<H1> There are two way of navigation using  fragments. Static and Dynamic. </H1></br>
<H2> For static: </H2> </br> use a fragment view in the activity_main.xml and the set the name attiribute with fragment object. 
<H2> For dynamic:  </H2> </br>use fragmentmanager, fragmentchannel.

<H1> send information in between fragments </H1>

```
Bundle bundle = new Bundle();
bundle.putString("key", "value");

MyFragment fragment = new MyFragment();
fragment.setArguments(bundle);

getSupportFragmentManager().beginTransaction()
        .replace(R.id.fragment_container, fragment)
        .commit();
```
