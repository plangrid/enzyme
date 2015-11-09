# `.filterWhere(predicate) => ShallowWrapper`

Returns a new wrapper with only the nodes of the current wrapper that, when passed into the 
provided predicate function, return true.


#### Arguments

1. `predicate` (`ReactElement => Boolean`): A predicate function to match the nodes.



#### Returns

`ShallowWrapper`: A new wrapper that wraps the filtered nodes.



#### Example

```jsx
const wrapper = shallow(<MyComponent />);
const complexFoo = wrapper.find('.foo').filterWhere(n => typeof n.type !== 'string');
expect(complexComponents).to.have.length(4);
```


#### Related Methods

- [`.filter(selector) => ShallowWrapper`](filter.md)