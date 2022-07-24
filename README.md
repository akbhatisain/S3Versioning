# S3Versioning
python script for Recovery from AWS S3 Versioning (Delete marker Data).
When you enable versioning on aws s3 bucket, in that case if any file got deleted, aws keep a copy of that. that file is in delete marker.
to recover all of the files back we need to remove delete marker file from bucket, and we will get original file back in bucket.
this is a manual process on console which take time in case of thousands files.

Here is the solution, with this python script we need to define bucket name, script will automatically remove all the delete marker.
Make sure versioning is enable on your bucket, it is a good feature from aws side.

This is tested script and works for me. Your case might be different, you can do some modification in script at your end.

Requirement:-
boto
boto-core
python latest version
aws cli configure with proper access on aws s3.

USAGE:
# python s3versioning-recovery.py
