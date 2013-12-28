At some point, it was decided that all the significant logic be exported to
supporting libraries. The MVCC logic grouped into a collection of libraries that
are linked by the `mvcc` project on NPM. Encoding and the the pair record
structure were also extracted into libraries that are separate from the MVCC
collection, they are specific to LevelDB while the MVCC collection can be used
to build other databases.

### Issue by Issue

 * Re-implement open using extracted libraries. #67.