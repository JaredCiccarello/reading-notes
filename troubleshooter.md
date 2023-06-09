'use strict'


Error: Request failed with status code 404
Solution: Changed .env and restarted .env several times and then waited.


Error: this.props.handleAddItem is not a function
Solution:
Child component: AddItem:  
handleSubmit = (e) => {
    e.preventDefault();
    this.props.handleAddItem(this.state.formData)
  }

Parent component: App :
<Form 
handleAddItem={this.addItem} 
/>


Error: Uncaught TypeError: Cannot read properties of undefined (reading 'map')
Solution:

In the child (items) component we have:  
              
              this.props.itemsList.map((item, idx) => <Item 
              key={item._id} 
              itemData={item} 
                />
              )

In the parent (app.js) component we have: 
              <Items 
              itemsList={this.state.itemsList} 
              should be 
              <Items 
              itemsList={this.state.items} 


Error: Cannot read properties of null (reading 'cats')
Solution: Ensure this.props.cats.map is being passed over properly using this.props. from parent file into the parent (App.js) into child (cats.js)

this.deleteItem.binds is not a function
Solution: binds needs to be bind

