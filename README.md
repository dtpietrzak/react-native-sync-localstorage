# react-native-localstorage
Non-Async Local Storage

## [Installation]
    npm install --save react-native-sync-localstorage

## [Usage]

### 1. Load stored values at beginning
    import localStorage from 'react-native-sync-localstorage'

    ...

    localStorage.getAllFromLocalStorage()
      .then(() => {
        // Do Something after loading...
      })
      .catch(err => {
        console.warn(err)
      })

### 2. Use local storage comfortably
#### 2-1. Setting
    const value = 12345
    localStorage.setItem('key', value)

#### 2-2. Getting
    localStorage.getItem('key')

#### 2-3. Deleting
    localStorage.removeItem('key')
