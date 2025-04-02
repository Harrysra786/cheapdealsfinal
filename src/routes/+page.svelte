<script>
    import { Button } from "$lib/components/ui/button";
    import { Card, CardContent, CardDescription, CardFooter, CardHeader, CardTitle } from "$lib/components/ui/card";
    import { Badge } from "$lib/components/ui/badge";
    import { Separator } from "$lib/components/ui/separator";
    import { ShoppingCart, Heart, Star, Plus, ArrowRight } from "@lucide/svelte";
  </script>
  
  <div class="grid grid-cols-1 md:grid-cols-5 gap-6 p-6">
    <!-- Card Design 1 - Simple and Clean -->
    <Card class="overflow-hidden transition-all hover:shadow-lg">
      <div class="aspect-square relative overflow-hidden bg-zinc-100">
        <img src="https://placehold.co/300x300" alt="Product" class="object-cover w-full h-full" />
      </div>
      <CardHeader class="p-4">
        <CardTitle class="text-lg">Modern Chair</CardTitle>
        <CardDescription class="font-medium text-zinc-900">$149.99</CardDescription>
      </CardHeader>
      <CardFooter class="p-4 pt-0">
        <Button class="w-full">
          <ShoppingCart class="mr-2 h-4 w-4" />
          Add to Cart
        </Button>
      </CardFooter>
    </Card>
  
    <!-- Card Design 2 - With Badge and Rating -->
    <Card class="overflow-hidden group">
      <div class="aspect-square relative overflow-hidden">
        <img src="https://placehold.co/300x300" alt="Product" class="object-cover w-full h-full transition-transform group-hover:scale-105" />
        <Badge class="absolute top-2 right-2 bg-zinc-900 text-white">New</Badge>
      </div>
      <CardHeader class="p-4">
        <div class="flex items-center gap-1 mb-1">
          <Star class="h-4 w-4 fill-zinc-500 text-zinc-500" />
          <Star class="h-4 w-4 fill-zinc-500 text-zinc-500" />
          <Star class="h-4 w-4 fill-zinc-500 text-zinc-500" />
          <Star class="h-4 w-4 fill-zinc-500 text-zinc-500" />
          <Star class="h-4 w-4 text-zinc-300" />
        </div>
        <CardTitle class="text-lg">Leather Backpack</CardTitle>
        <div class="flex justify-between items-center mt-1">
          <CardDescription class="font-bold text-zinc-900">$89.99</CardDescription>
          <Button size="sm" variant="outline" class="rounded-full h-8 w-8 p-0">
            <Heart class="h-4 w-4" />
          </Button>
        </div>
      </CardHeader>
      <CardFooter class="p-4 pt-0">
        <Button class="w-full" variant="secondary">Buy Now</Button>
      </CardFooter>
    </Card>
  
    <!-- Card Design 3 - Elegant with Separator -->
    <Card class="overflow-hidden border-none shadow-md hover:shadow-xl transition-shadow">
      <div class="aspect-square relative overflow-hidden bg-zinc-50">
        <img src="https://placehold.co/300x300" alt="Product" class="object-cover w-full h-full" />
      </div>
      <CardContent class="p-6">
        <CardTitle class="text-lg mb-1">Minimalist Watch</CardTitle>
        <CardDescription class="text-zinc-500 mb-3">Premium Collection</CardDescription>
        <Separator class="my-3" />
        <div class="flex justify-between items-center">
          <span class="text-lg font-semibold">$199.99</span>
          <Button variant="ghost" size="icon" class="rounded-full">
            <Plus class="h-4 w-4" />
          </Button>
        </div>
      </CardContent>
      <CardFooter class="px-6 pb-6 pt-0">
        <Button class="w-full bg-zinc-900 hover:bg-zinc-800 text-white">Add to Cart</Button>
      </CardFooter>
    </Card>
  
    <!-- Card Design 4 - Modern with Hover Effect -->
    <Card class="group relative overflow-hidden border-0 shadow-sm hover:shadow-md transition-all">
      <div class="absolute inset-0 bg-gradient-to-t from-zinc-900/70 to-transparent opacity-0 group-hover:opacity-100 transition-opacity z-10"></div>
      <div class="aspect-square relative overflow-hidden">
        <img src="https://placehold.co/300x300" alt="Product" class="object-cover w-full h-full" />
      </div>
      <div class="absolute bottom-0 left-0 right-0 p-4 z-20 translate-y-4 opacity-0 group-hover:translate-y-0 group-hover:opacity-100 transition-all">
        <CardTitle class="text-white text-lg mb-1">Wireless Earbuds</CardTitle>
        <div class="flex justify-between items-center">
          <CardDescription class="text-white font-bold">$129.99</CardDescription>
          <Button size="sm" variant="secondary" class="bg-white text-zinc-900 hover:bg-zinc-100">
            Buy Now
          </Button>
        </div>
      </div>
      <CardHeader class="p-4 group-hover:opacity-0 transition-opacity">
        <CardTitle class="text-lg">Wireless Earbuds</CardTitle>
        <CardDescription class="font-bold text-zinc-900">$129.99</CardDescription>
      </CardHeader>
    </Card>
  
    <!-- Card Design 5 - Horizontal Layout -->
    <Card class="overflow-hidden flex flex-col md:flex-row">
      <div class="w-full md:w-1/2 aspect-square md:aspect-auto relative overflow-hidden bg-zinc-100">
        <img src="https://placehold.co/300x300" alt="Product" class="object-cover w-full h-full" />
      </div>
      <div class="w-full md:w-1/2 flex flex-col p-4">
        <CardTitle class="text-lg mb-2">Smart Speaker</CardTitle>
        <CardDescription class="text-zinc-500 mb-2 flex-grow">Voice controlled with premium sound</CardDescription>
        <div class="mt-auto">
          <div class="text-lg font-bold mb-3">$79.99</div>
          <Button class="w-full flex items-center justify-center gap-1">
            Shop Now
            <ArrowRight class="h-4 w-4" />
          </Button>
        </div>
      </div>
    </Card>
  </div>
  