
# lists with RecyclerView 

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQO-B3UGj4LIQCItbAq1fBs_7njZSy5gPLkyw&usqp=CAU)

RecyclerView: 

 is the ViewGroup that contains the views corresponding to your data. it is useful for making it easy to efficiently display large sets of data. It improves performance, 
improves the responsiveness, and reduces power consumption. 


When an item scrolls off something it doesn't destroy its view, but  reuses the view for new items that have scrolled on. 

building a dynamic list: 
Several classes work together to build it, 

- RecyclerView
A flexible view for providing a limited window into a large data set.

1. Adapter, responsible for providing views that represent items in a data set. 
`RecyclerView.Adapter`
2. The position of a data item within an Adapter.
 types of position:

 - layout position 
 - adapter position 

3. The index of an attached child view as used in a call to
`ViewGroup.getChildAt(int)`
4. Binding and preparing a child view to display data corresponding to a position within the adapter.
5. Recycle (view): A view previously used to display data for a specific adapter position may be placed in a cache for later reuse to display the same type of data again later

6. Scrap (view): A child view that has entered into a temporarily detached state during layout. 
7. Dirty (view): A child view that must be rebound by the adapter before being displayed. 

-  view holder object.
`RecyclerView.ViewHolder`
it doesn't have any data associated with it. After the view holder is created, the RecyclerView binds it to its data

-  Adapter,responsible for providing views that represent items in a data set. 
`RecyclerView.Adapter`  

- The layout manager  `LayoutManager`


## implementing  RecyclerView

- Plan your layout 
1. LinearLayoutManager 
2. GridLayoutManager 
3. StaggeredGridLayoutManager 

- Implementing your adapter and view holder (binding)

`ViewHolder` is a wrapper around a View that contains the layout for an individual item in the list.

` Adapter` creates ViewHolder objects as needed, and also sets the data for those views.



