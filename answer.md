Question: Which out of the two components (which are performing the same functionality) is performing better and how?


Answer:

The purecomponent rendered by PureCounter.jsx, is performing better compared to the one rendered by SimpleCounter.jsx, because of the usage of PureComponent class, which has been imported from React.

Since the PureCounter class in Purecounter.jsx extends to PureComponent, **PureCounter component is rendered only if the props** (which in this case are **"toggle"** and **"count"**) **are changed.**
Whereas the SimpleCounter component will rerender, even if the props are not changed.

Thus **PureComponent gets rid of unneccessary renders**, by checking if props are changed or not.
