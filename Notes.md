<h2>10.04.2024</h2>
<p>Since I want to use two separate databases (SQL Server for tests and a PostgreSQL for users), I am currently in a process of learning how to properly integrate both databases into EF Core.</p>
<p>Currently, I have done following:</p>
<ul>
  <li>Created an SQL Server Database for tests</li>
  <li>Added Models folder</li>
  <li>Added TestType model</li>
  <li>Added Test model</li>
  <li>Added Question model</li>
  <li>Added AnswerOption model</li>
  <li>Added tables into the Database that are corresponding to the models above (with Migration and an Update) while using code first approach</li>
</ul>
<p>Also, I have learned more about such things as DTO and Mapper so I decided to add them into a backend project as well.</p>
<p>Made a Github repository initialization and after that few pushes as well.</p>

<h2>11.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Repository Pattern</li>
  <li>Dependency Injection</li>
  <li>Logging via Serilog</li>
  <li>How to add an SQLite database (later to be used for storing logging information.)</li>
  <li>How to implement global exception handling middleware</li>
  <li>Process of overriding ToString() method with JsonSerializer.Serialize(this)</li>
</ul>

<h2>12.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>How to make my controller action methods more maintainable through:</li>
  <ol>
    <li>Repository Pattern</li>
    <li>DTos</li>
    <li>Mapping</li>
    <li>Exception Handling</li>
    <li>Action Filters</li>
    <li>Tight Coupling</li>
  </ol>
  <li>Filters (Action Filter)</li>
  <li>ServiceFilter, TypeFilter (if arguments are required), IActionFilter</li>
</ul>

<h2>14.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Get by id route</li>
  <li>Create route with a [FromBody] attribute</li>
  <li>Delete route</li>
  <li>HttpContent for HTTP requests</li>
  <li>CreatedAtAction</li>
  <li>Using mapper for updating an entity</li>
</ul>

<h2>15.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Difference between HttpPut and HttpPatch (Patch can be used for a partial update which in return can reduce a payload that is required to send. Put is used to create an entirely new object or update an already existing object fully)</li>
</ul>

<p>Did following:</p>
<ul>
  <li>Added interface for a Test repository</li>
  <li>Added repository for a Test entity</li>
  <li>Added Test controller</li>
</ul>

<p>Got introduced with an object cycle during JSON serialization.</p>
<p>Fixed it by adding a [JsonIgnore] attribute that will ignore my navigation property in a Test entity.</p>
<p>Added JsonPatchDocument for patch route support.</p>
<p>Fixing/fixed following problems:</p>
<ul>
  <li>The instance of entity type 'Test' cannot be tracked because another instance with the same key value for {'TestID'} is already being tracked. When attaching existing entities, ensure that only one entity instance with a given key value is attached. Consider using 'DbContextOptionsBuilder.EnableSensitiveDataLogging' to see the conflicting key values.</li>
  <li>An unhandled exception has occurred while executing the request. System.Text.Json.JsonException: A possible object cycle was detected. This can either be due to a cycle or if the object depth is larger than the maximum allowed depth of 32.</li>
</ul>

<h2>16.04.2024</h2>
<p>Found out about .NET Aspire.</p>

<h2>17.04.2024</h2>
<p>Currently learning if a null is a desired data type to return as a result.</p>
<p>So far, it seems better to return an empty array if method is designed to return an array or list.</p>
<p>When talking about a method that returns a single item, there are a lot of options. For now, I will stick with returning null in my repository and then handle that in my action method.</p>
<p>Using FirstOrDefault() or Find() when looking for an object by using and id. Find() can skip making a request into a database since it will track if this id was already used somewhere else.</p>

<h2>19.04.2024</h2>
<p>Learning about authentication and authorization in ASP .NET Core.</p>
