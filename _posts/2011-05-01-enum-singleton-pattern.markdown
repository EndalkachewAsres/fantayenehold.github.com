---
layout: post
title: Enum Singleton Pattern
permalink: /2011/05/enum-singleton-pattern/
---

Here it is how you can create a singleton UTILITY class.

	public interface UnaryFunction<T> { 
		T apply(T arg);
	}
	
	public enum IdentityFunction implements UnaryFunction<Object> {
		INSTANCE;
		
		public Object apply(Object arg) { return arg; }
	}

	

