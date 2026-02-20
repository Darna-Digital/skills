# React

## Imports

1. Prefer useState instead of React.useState, same for other React hooks.


## Props

1. Don't use named props, just call them Props.

So no:

```
type RemoveInternalProjectDialogProps = {
    isOpen: boolean;
};

export function RemoveInternalProjectDialog({isOpen}: RemoveInternalProjectDialogProps) {}
```

Instead use:

```
type Props = {
    isOpen: boolean;
};

export function RemoveInternalProjectDialog({isOpen}: Props) {}
```

