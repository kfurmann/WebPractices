css DPI

To apply a style sheet to devices with at least 300 dots per inch of resolution:

@media print and (min-resolution: 300dpi) { ... }

Change CSS with js:

document.getElementById('id').style.width = value;


Inheritance (kind of) http://yehudakatz.com/2011/08/12/understanding-prototypes-in-JavaScript/

var child = Object.create(parent);

better:

var Person = function(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}
 
Person.prototype = {
  toString: function() { return this.firstName + ' ' + this.lastName; }
}

var mark = new Person("Mark", "Miller");
mark.toString() // "Mark Miller"