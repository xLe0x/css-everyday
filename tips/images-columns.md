Ever wondered how to make this?

![An image contains 3 columns of images](./images/images-columns.png)

sounds hard right?

not any more with `columns` property!


let's see the result without using `columns` property 

```html
    <div class="container">
      <img
        width="300px"
        src="https://images.unsplash.com/photo-1742129726461-ea9c742d3860?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDJ8NnNNVmpUTFNrZVF8fGVufDB8fHx8fA%3D%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://plus.unsplash.com/premium_photo-1674086524511-567ad049a61a?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDF8NnNNVmpUTFNrZVF8fGVufDB8fHx8fA%3D%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://plus.unsplash.com/premium_photo-1712685912274-2483dade540f?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDR8NnNNVmpUTFNrZVF8fGVufDB8fHx8fA%3D%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://images.unsplash.com/photo-1741926376117-85ec2cef9714?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDZ8NnNNVmpUTFNrZVF8fGVufDB8fHx8fA%3D%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://images.unsplash.com/photo-1741877649919-4619ae378927?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDEwfDZzTVZqVExTa2VRfHxlbnwwfHx8fHw%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://images.unsplash.com/photo-1741800459656-4116dcb230ae?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDE0fDZzTVZqVExTa2VRfHxlbnwwfHx8fHw%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://plus.unsplash.com/premium_photo-1673618856293-87849f06ffaf?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDIzfDZzTVZqVExTa2VRfHxlbnwwfHx8fHw%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://plus.unsplash.com/premium_photo-1673120765126-066ad8fedc9d?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDM1fDZzTVZqVExTa2VRfHxlbnwwfHx8fHw%3D"
        alt=""
      />
      <img
        width="300px"
        src="https://plus.unsplash.com/premium_photo-1700346373090-151ac589b07d?w=300&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHx0b3BpYy1mZWVkfDM5fDZzTVZqVExTa2VRfHxlbnwwfHx8fHw%3D"
        alt=""
      />
    </div>
```

```css
 .container {
    width: min(1000px, 100%); /* not required */
    margin: 0 auto; /* not required */
}
```

this is the result:

![](./images/images-columns-bad.png)

what if we added this line?

```css
 .container {
    width: min(1000px, 100%); /* not required */
    margin: 0 auto; /* not required */
    columns: 3 300px;
}
```

now:

![](./images/images-columns-column-added.png)

gaps looks bad?

use `column-gap: 1rem` to add gaps of 1rem between each column!

row gaps aren't equal? remeber that images are inline elements and that means they are affected by `line-height`! [Refere to MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#styling_with_css)

so we should fix this:

```css
img {
    display: block;
    margin-bottom: 1rem; /* to match the column gap! */
    width: 100%;
}
```
