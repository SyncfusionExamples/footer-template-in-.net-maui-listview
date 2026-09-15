# Footer template in NET MAUI ListView (SfListView)

This example demonstrates about how to show the items count in Footer view of .NET MAUI ListView (SfListView).

## Sample

```xaml
<listView:SfListView x:Name="listView" ItemSize="70"
                                 GroupHeaderSize="60" 
                                 FooterSize="60" ItemSpacing="0" IsStickyFooter="True"
                                 ItemsSource="{Binding Items}">

    <listView:SfListView.FooterTemplate>
        <DataTemplate>
            <StackLayout Orientation="Horizontal" HorizontalOptions="Start" 
                                VerticalOptions="Center" Padding="10,0,0,0">
                <Label Text="Items Count" TextColor="Black" FontSize="Medium"/>
                <Label Text="{Binding Items.Count}" TextColor="Black" FontSize="Medium"/>

            </StackLayout>
        </DataTemplate>
    </listView:SfListView.FooterTemplate>

    <listView:SfListView.ItemTemplate>
        <DataTemplate>
            <StackLayout>
                <Label Text="{Binding ContactName}" FontSize="20"/>
                <Label Text="{Binding ContactNumber}" FontSize="15"/>
            </StackLayout>
            
        </DataTemplate>
    </listView:SfListView.ItemTemplate>

</listView:SfListView>
```

## Requirements to run the demo

* [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) or [Visual Studio for Mac](https://visualstudio.microsoft.com/vs/mac/)
* Xamarin add-ons for Visual Studio (available via the Visual Studio installer).

## Troubleshooting

### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

