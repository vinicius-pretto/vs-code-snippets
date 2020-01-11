# Visual Studio Code Snippets

## React

* imr (Import React) 

```
import React from 'react';
```

* exd (Export default component)

```
export { default } from './$1';
```

* rcc (React class component)

```
import React from 'react';
import styled from 'styled-components';

const $1 = styled.$2`
  $4
`;

class $3 extends React.Component {
  render() {
    return (
      <$1>$5</$1>
    )
  }
}

export default $3;
```

* rsc (React stateless component)

```
import React from 'react';
import styled from 'styled-components';

const $1 = styled.$2`
  $4
`;

const $3 = () => {
  return (
    <$1>$5</$1>
  )
};

export default $3;
```

## Storybook

* stb (Storybook default)

```
import React from 'react';
import { storiesOf } from '@storybook/react';

import $1 from './$1';

storiesOf('$2', module).add('default', () => (
  <$1></$1>
));
```

* stbc (Storybook core components)

```
import React from 'react';
import { storiesOf } from '@storybook/react';

import $1 from './$1';

storiesOf('components/core/$1', module).add('default', () => (
  <$1>$2</$1>
));
```

## Jest

* jst (Jest create snapshot test)

```
import React from 'react';
import '@testing-library/react';

import $1 from './$1';

describe('$1', () => {
  it('snapshot', () => {
    const { asFragment } = renderWithTheme(
      <$1>$2</$1>
    );
    expect(asFragment()).toMatchSnapshot();
  });
});
```

* desc (Describe block) 

```
describe('$1', () => {
  it('$2', () => {
    $3
  });
});
```

* it (It block)

```
it('$1', () => {
  $2
});
```
