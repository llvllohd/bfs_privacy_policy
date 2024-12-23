# SonicPlatform MSW MicroApp

> Unified UI Template to help you set up the initial UUIF project quickly

## Steps

> Whenever you are adding a new component make sure to hide/show breadcrumb using [isMicroAppMode] getter which is in core store.
	we have to hide breadcrumb while running an App as a SubApp and show it while running as a monolithic.

> While calling an apis use [apiConfiguredService] which is an ApiServiceWrapper from `shared/msw-api-service` folder.
	please donot use from spwc-api-service folder as it will be removed in the future.

> For fetching [CSRF] token use [retrieveCsrfToken] function from session keeper service which is in `shared/session-keeper-service` folder.

> For fetching [UserDetails] such as email, userId, roles, orgId, sessionId use data keeper service which is in `shared/data-keeper-service` folder.
