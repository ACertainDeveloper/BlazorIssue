# Blazor Issue
Repository demonstrating an issue with a blazor component in a razor view layout page.

# Description
A blazor component works fine in a razor layout page (a menu for example).

'''c#
 @(await Html.RenderComponentAsync<MyComponent>(RenderMode.ServerPrerendered))
'''

If a blazor component is included in a razor page that uses the layout, both componets fail to function. The browser console gives follwing errors: 
* Error: The list of component records is invalid.
* Information: Connection disconnected.
* Error: Invocation canceled due to the underlying connection being closed