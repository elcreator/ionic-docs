```tsx
import React from 'react';
import { IonContent, ScrollDetail } from '@ionic/react';

function Example() {
  function handleScrollStart() {
    console.log('scroll start');
  }

  function handleScroll(event: CustomEvent<ScrollDetail>) {
    console.log('scroll', JSON.stringify(event.detail));
  }

  function handleScrollEnd() {
    console.log('scroll end');
  }

  return (
    // Scroll events are disabled by default for content for performance reasons, enable them to listen to them
    <IonContent
      scrollEvents={true}
      onIonScrollStart={handleScrollStart}
      onIonScroll={handleScroll}
      onIonScrollEnd={handleScrollEnd}
      class="ion-padding"
    >
      <h1>Scroll to fire the scroll events and view them in the console.</h1>

      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean sed tellus nec mauris auctor dignissim fermentum
        in risus. Sed nec convallis sapien, id tincidunt enim. Mauris ornare eleifend nunc id mattis. Fusce augue diam,
        sagittis nec posuere at, consectetur tempor lectus. Nulla at lectus eget mauris iaculis malesuada mollis sed
        neque. Curabitur et risus tristique, malesuada mauris finibus, elementum massa. Proin lacinia mauris quis ligula
        blandit ullamcorper. Donec ut posuere lorem. In volutpat magna vitae tellus posuere pulvinar. Nam varius ligula
        justo, nec placerat lacus pharetra ac. Aenean massa orci, tristique in nisl ut, aliquet consectetur libero.
        Etiam luctus placerat vulputate. Aliquam ipsum massa, porttitor at mollis ut, pretium sit amet mi. In neque
        mauris, placerat et neque vel, tempor interdum dolor. Suspendisse gravida malesuada tellus, vel dapibus nisl
        dignissim vel. Cras ut nulla sit amet erat malesuada euismod vel a nulla.
      </p>
      <p>
        Phasellus sit amet iaculis odio, eget feugiat erat. Etiam sit amet turpis sit amet massa viverra maximus. Aenean
        venenatis porttitor pharetra. Fusce vulputate urna purus, vel efficitur mauris auctor non. Etiam libero odio,
        sodales in velit a, faucibus venenatis erat. Ut convallis sit amet urna in ultrices. Cras neque est, vehicula
        sed lorem ac, placerat commodo elit. Praesent turpis metus, elementum eget iaculis ac, elementum in odio. Nunc
        et elit faucibus, condimentum mauris consequat, ornare dolor. Sed ac lectus a est blandit tempor. Etiam lobortis
        tristique maximus.
      </p>
      <p>
        Quisque tempus porttitor massa, vel condimentum risus finibus a. Aliquam viverra maximus odio, id ornare justo
        tristique ac. Mauris euismod arcu eget neque sagittis rutrum. Ut vehicula porta lacus nec lobortis. Vestibulum
        et elit ultrices, lacinia metus in, lobortis est. Vivamus nisi justo, venenatis sit amet arcu ac, congue
        faucibus justo. Duis volutpat posuere enim, vel sagittis elit dictum et. Sed et congue mauris. Nam venenatis
        venenatis risus, ac condimentum neque sagittis sed. In eget nulla ultricies urna sollicitudin posuere. Aenean
        sagittis congue mauris. Proin nec libero mi. In hac habitasse platea dictumst. Praesent nunc nulla, dictum id
        molestie sed, pretium vitae turpis.
      </p>
      <p>
        Pellentesque vitae dapibus lacus. Nullam suscipit ornare risus quis ullamcorper. Nullam feugiat, sapien et
        sodales fermentum, risus ligula semper risus, id efficitur ligula augue id diam. Suspendisse lobortis est sit
        amet quam facilisis, ut vestibulum nunc dignissim. Donec at vestibulum magna. Maecenas maximus pretium metus.
        Phasellus congue sapien vel odio imperdiet, nec mollis odio euismod. Sed vel eros ut sapien accumsan condimentum
        vehicula vitae lectus. Donec sed efficitur lorem. Aenean tristique mi libero, eleifend tincidunt libero finibus
        at. Mauris condimentum fermentum rutrum.
      </p>
      <p>
        Nulla tristique ultricies suscipit. Donec non ornare elit. Vivamus id pretium mauris, nec sagittis leo. Fusce
        mattis eget est id sollicitudin. Suspendisse dictum sem magna, in imperdiet metus suscipit et. Suspendisse enim
        enim, venenatis et orci eu, suscipit congue lacus. Praesent vel ligula non eros tempor interdum. Proin justo
        orci, ultricies vitae diam sed, semper consectetur ligula. Aenean finibus ante velit, nec efficitur libero
        cursus cursus. Duis mi nunc, imperdiet sed condimentum vel, porttitor ut lacus. Quisque dui ipsum, vehicula sed
        vestibulum id, semper vel libero. Suspendisse tincidunt mollis condimentum. Nulla facilisi. Etiam neque nisl,
        egestas nec iaculis sed, tristique faucibus sem. Sed mollis dui quis ligula cursus rutrum.
      </p>
    </IonContent>
  );
}
export default Example;
```
