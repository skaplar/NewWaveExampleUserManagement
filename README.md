# NewWaveExampleUserManagement
This is an example user management that contains files which can be used as a guidance.

## Usage

You can use these files inside of engine, to specify roles. You can use these files with the NWUserManagement class.

```smalltalk

| management |

management := NWUserManagement 				  						   
		pathToUsers:'/Users/sebastijan.kaplar/Desktop/NewWave-JobPosting-Management/users.json'
		pathToGroups: '/Users/sebastijan.kaplar/Desktop/NewWave-JobPosting-Management/groups.json'
		pathToMemberships: '/Users/sebastijan.kaplar/Desktop/NewWave-JobPosting-Management/membership.json'.
```

And then while creating an engine you can pass it the newly created user management.

```smalltalk

engine := WaveEngine new.
engine loadUsersAndGroups: management.

```
