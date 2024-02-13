# @charlybourgouin/p14_modal_component
`p14_modal_component` is a lightweight React library for creating simple modals.

# react-simple-modal

`react-simple-modal` is a lightweight React library for creating simple modals.

## Installation

Install the library via npm:

```bash
npm install @charlybourgouin/p14_modal_component
```

## Usage

```jsx
import { useState } from 'react';
import Modal from '@charlybourgouin/p14_modal_component';

function App() {
  const [modalOpen, setModalOpen] = useState(false);

  return (
    <div>
      {/* Your main content here */}
      <Modal text="Modal content" modalOpen={modalOpen} setModalOpen={setModalOpen} />
    </div>
  );
}

export default App;

```

## Props

### ```text``` (String, required)
The text to be displayed inside the modal.

### ```modalOpen``` (Boolean, required)
A boolean indicating whether the modal is open or closed.

### ```setModalOpen``` (Function, required)
A function to toggle the modal state.

## Custom Styles

You can customize the style of the modal using style properties by passing an object as the style prop.

## Full Example

```jsx
import { useState } from 'react';
import Modal from 'p14_modal_component';

function App() {
  const [modalOpen, setModalOpen] = useState(false);

  return (
    <div>
      {/* Your main content here */}
      <Modal
        text="Modal content"
        modalOpen={modalOpen}
        setModalOpen={setModalOpen}
        // You can add custom styles here
      />
    </div>
  );
}

export default App;


```