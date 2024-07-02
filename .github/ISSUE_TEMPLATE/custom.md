---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: bug, documentation, duplicate, enhancement, good first issue, help wanted,
  invalid, question, wontfix
assignees: Playgirlkaybraz11

---

import { Devvit } from '@devvit/public-api';
import { Columns } from '@devvit/kit';

Devvit.addCustomPostType({
  name: 'Columns static content',
  render: () => {
    return (
      <vstack padding="medium">
        <Columns columnCount={2} gapX="5px" gapY="10px" order="column">
          <hstack backgroundColor="grey">
            <text>Birds</text>
          </hstack>
          <hstack>
            <text>Raven</text>
          </hstack>
          <hstack>
            <text>Parrot</text>
          </hstack>

          <hstack backgroundColor="grey">
            <text>Dogs</text>
          </hstack>
          <hstack>
            <text>Bulldog</text>
          </hstack>
          <hstack>
            <text>Poodle</text>
          </hstack>
        </Columns>
      </vstack>
    );
  },
});
