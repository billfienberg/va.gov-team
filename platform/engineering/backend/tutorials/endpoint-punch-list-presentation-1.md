# endpoint-punch-list-presentation

## Vets-API Endpoint Punch List Presentation

### Presentation

* [Video presentation](https://www.youtube.com/watch?v=V_i8JLXk5rg)
* [view slides](https://hackmd.io/@z9SepQsSSlu0NKymVGnXTA/r1ZdSNJmr#/) \(view\)
* [edit slides](https://hackmd.io/FdnzysLHRD2BuKostPBUxw?both)

=======================

### Source File

\(this is a versioned backup of the slides in hackmd\)

slideOptions: transition: slide slideNumber: true

 \# Endpoint Punch List

 \# Endpoint Code

 \# Swagger Docs

 \# Betamocks

 \# Spec Coverage

## Frontend Signoff

```javascript
{
  "data": {
    "attributes": {
      "email": "john@example.com",
      "effective_at": "2018-02-27T14:41:32.283Z"
    }
  }
}
```

:white\_check\_mark: :white\_check\_mark: :white\_check\_mark:

## Endpoint Code

## Endpoint Creation

* Integrate an external service
* Service object
* Controller, route and serializer

## Service Object

* Calls the service's endpoints
* Dependencies
  * Service class
  * Config class & Faraday connection
  * Response class
  * settings.yml

### [Service Object Implementation](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/service-object-implementation.md)

### [Controller/Route/Serializer](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/controller-route-serializer.md)

## Swagger Docs

 \#\# Request/Response Docs

 \#\# Model Docs

## Swagger Files

```bash
app/swagger/requests/*
```

```bash
app/swagger/schemas/*
```

```bash
app/controllers/v0/apidocs_controller.rb
```

[Swagger implementation](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/swagger-impementation.md)

## Betamocks

## Betamocks Process

1. Set config
2. Create recording
3. Update mock data table

### [Betamocks Config](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/betamocks-config.md)

### [Betamocks Recording & Mock Data Table](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/betamocks-recording-mock-data-table.md)

## Spec Coverage

## Spec Areas

* Service object specs
* Request specs
* VCR cassettes
* Response schema
* [Spec files examples](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/spec-files-examples.md)

### `match_response_schema`

```ruby
expect(response).to match_response_schema(
  'email_address_response'
)
```

#### [`match_response_schema` Implementation](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/platform/engineering/backend/tutorials/endpoint-punch-list-presentation/supporting_code/match_response_schema-implementation.md)

## In Conclusion

 \#\# \[Endpoint Punch List\]\(\)

## Resources

* [Integrate an external service](https://github.com/department-of-veterans-affairs/devops/tree/master/docs/External%20Service%20Integrations)
* [Email address endpoint PR](https://github.com/department-of-veterans-affairs/vets-api/pull/1718)
* [Email address Betamocks config PR](https://github.com/department-of-veterans-affairs/vets-api/pull/1746)
* [Email address Betamocks recording PR](https://github.com/department-of-veterans-affairs/vets-api-mockdata/pull/13)
* [Setup Swagger locally](https://github.com/department-of-veterans-affairs/vets-api/tree/master/app/swagger)
* [Setup Betamocks](https://github.com/department-of-veterans-affairs/vets-api/blob/master/docs/setup/betamocks.md)
* [vets-api-mockdata readme](https://github.com/department-of-veterans-affairs/vets-api-mockdata/blob/master/README.md)
* [Endpoint Punch List](endpoint-punch-list-presentation-1.md)

## Questions?

## Q & A Takeaways

* get the API correct, collaborate with the architects
* dealing smartly and proactively with the error edge cases
* insight into how the middleware is being instrumented, and references to them
* alphabetize the Swagger API endpoints
* automate the inclusion of the files in the apidocs controller

## Thanks!

