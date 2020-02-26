# Problem with permissions when copying files from CBS RA to OSSC with WinSCP
```
When trying to copy data using WinSCP, the transfer will almost complete but then fails with an error:

    Upload of file 'test.gz' was successful, but error occurred while setting the permissions and/or timestamp
    Permission denied, error code:3 error message from server: Permission denied.

Subsequently i do have read access to the copied files on OSSC. Additionally i have access to make, delete directories. Create files using vi.

However extracting the zips and gzips transferred fails due to permissions error.

tar -zxvf biogeme-2.5.tar.gz creates the directory biogeme-2.5 but it will not extract any files into it, as it's fails due to a lack of permission.
```


We need more time to solve this issue.

For the time being I would like to ask you to login as user ossc9997 from the CBS RA, so in the putty profile and winscp profile change your username for the time being. You should be accepted by the system as that user as well.


