# Simple c++ thread pool

### usage

Create a threadpool which contains 32 threads:

```
ThreadPool* threadpool = new ThreadPool(32);
```

Add a function func(arg1, arg2,...,argn) to task queue:

```
threadpool->addTask(func,arg1,arg2,...,argn);
```

Add a non-static member function of class C to task queue:

```
threadpool->addTask(&C::func,instance_of_C,arg1,arg2,...,argn);
```
