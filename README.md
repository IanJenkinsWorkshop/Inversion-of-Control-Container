# IOC Container ( Inversion Of Control )

<h1>Inversion of Control Container ( IOC )</h1>

<p>This is a very basic light weight container. </p>

<p>Instead of installing a full blooded framework to provide a container to handle inversion of control you can use this light weight very small container.<p/>

<p>

<h2> Description </h2>

<p>To setup the container you must first register all your dependencies. </p>

<h3>Step 1 -> Create the container instance.</h3>

<p>var ioc = new IoC();</p>

<h3>Step 2 -> Add dependency.</h3>

<p>you can either do it like this using an interface</p>

ioc.Add< IMadeUpObject, MadeUpObject >();

<h3>Add a Singleton</h3>

<p>ioc.AddSingleton< MadeUpObject >()</p>

<h3>Step 3 -> To implement an instance you do this.</h3>

<p>var obj = ioc.Get< IMadeUpObject >();</p>

<p>or</p>

<p>var obj = ioc.Get(typeof(MadeUpObject));</p>

