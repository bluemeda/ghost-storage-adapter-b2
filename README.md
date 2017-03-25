# Ghost Storage Adapter - Backblaze(B2) Cloud
This library works with current version of Ghost 0.11+

## Installation

Via NPM
```
npm install ghost-storage-adapter-b2
mkdir -p ./content/storage
cp -r ./node_modules/ghost-storage-adapter-b2 ./content/storage/b2
```

Via GIT
```
mkdir -p ./content/storage/b2
cd content/storage/b2
git clone git@github.com:martiendt/ghost-storage-adapter-b2.git .
npm install
```

## Configuration
Add this in `config.js` file
```
storage: {
    active: 'b2',
    'b2': {
        accountId: 'YOUR_ACCOUNT_ID',
        bucketId: 'YOUR_BUCKET_ID',
        bucketName: 'YOUR_BUCKET_NAME',
        key: 'YOUR_APPLICATION_KEY'
    }
}   
```

If you don't have an account, you can create your account [here](https://www.backblaze.com) and then create your bucket.

