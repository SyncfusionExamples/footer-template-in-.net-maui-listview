# footer-template-in-.net-maui-listview
This example demonstrates about how to show the items count in Footer view of .NET MAUI ListView (SfListView).

You can show items count in footer of ListView by directly binding the count property of ItemsSource bind with ListView.

```
<listView:SfListView.FooterTemplate>
    <DataTemplate>
        <StackLayout Orientation="Horizontal" HorizontalOptions="Start" 
                         VerticalOptions="Center" Padding="10,0,0,0">
            <Label Text="Items Count" TextColor="Black" FontSize="Medium"/>
            <Label Text="{Binding Items.Count}" TextColor="Black" FontSize="Medium"/>

        </StackLayout>
    </DataTemplate>
</listView:SfListView.FooterTemplate>
